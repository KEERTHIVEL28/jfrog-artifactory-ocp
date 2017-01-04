# jfrog-artifactory-ocp
An OpenShift Template for JFrog Artifactory

# Usage
As project user:

`oc create -f https://raw.githubusercontent.com/benemon/jfrog-artifactory-ocp/master/artifactory-template.yaml`

`oc new-app --template=artifactory-persistent`

Deployment will (probably) fail. If it does, as admin:

`oc adm policy add-scc-to-user anyuid -z artifactory-sa`
