A Deployment in Kubernetes is a higher-level abstraction over a ReplicaSet that provides additional functionality and features to manage the lifecycle of applications more effectively. It manages a set of identical pods, ensuring they run and scale as needed.

Deployment offers a more sophisticated way to manage the entire lifecycle of those pods, including updates, rollbacks, and scaling, providing a higher level of abstraction and more powerful features.
In this example, we have illustrated the relationship between a Deployment, a ReplicaSet, and its controlled replicas.

Task: Create a Kubernetes Deployment object:
Create a Deployment named nginx-deployment that uses the nginx:latest image with three replicas.

Declarative Approach
Install vim to edit/create the deployment menifest:
sudo apt update
sudo apt install vim

Create and open a yaml file for deployment definition:

vim deployment-definition.yaml

Here our file name is deployment-definition.yaml.

Here is a YAML menifest file. This YAML defines a Kubernetes Deployment named "nginx-deployment" that ensures three replicas of the nginx container are running, each exposing port 80.