# deploy on ocp

Currently, dify does not work well with no-root deployment, so we need to fix on that.

Apply the `scc.yaml` first, it will create scc and apply to the service account.

Then apply the `dify-ocp-deployment.yaml` to deploy dify.

2 components of dify need storage to support RWX, if your default storage class does not support RWX, you can try storage from ODF or NFS.

Here, we provide another example to deploy dify with storage from ODF, under `with.odf` folder.

# end
