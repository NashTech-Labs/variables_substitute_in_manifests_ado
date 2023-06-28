# variables_substitute_in_manifests_ado
We are changing the variables before the actual deployment of manifests into the Kubernetes cluster. In this, we are using Kubernetesmanifests@1 render kustomize. 
 1. Kubernetesmanifests@1 is a task in Azure DevOps that helps bake, deploy, and delete the pod.
 2. We can pass the variables using the kustomize render in the task by adding the PowerShell script task as in the azure-pipeline.yml
 3. The resulting manifests can be checked in a render.yaml
