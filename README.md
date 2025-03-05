# konflux-ci
Project holding the resources required to use Konflux as CI/CD system 

# RBAC extension

Pipelines are executed with SA `appstudio-pipeline` and as it will use mapt to dynamic provision envs we 
need to extend the permissions for the SA to allow create secrets.

# Raw 

To easily work agaisnt konflux-ci. We templated the config file under .kube with name `konflux-config` so then
we can interact with the cluster using: `kubectl --kubeconfig ~/.kube/konflux-config get application`


## podman-desktop-extension-macadam

Create initial resources for `podman-desktop-extension-macadam` on Konflux

`kubectl --kubeconfig ~/.kube/konflux-config apply -f  podman-desktop-extension-macadam/application.yaml`



