### first_app
* create_pods.yml creates a basic POD definition for a defined docker container. We use kubectl expose to view the application.
* loadbalancer.yml is a loadbalancer service which was used to integrate AWS elastic load balancer to our application.We can then use the DNS name created with ELB to point to our customized domain name using route 53.

### Replication Controllers
* rc.yml is used to create and control pod replicas based on the definition. We can then use this to scale up and down based on
requirements.RC basically work on the concept of a desired state, so if one of the pods fail rc brings it up.

### deployments/replica sets
* Deployments is in beta version while making this file. But deployments make it really easier for us to create pods and then scale them
automatically. 
* So essentially it creates a deployment object where we can give our definition of desired state and hence makes it easier to create,update, do rolling updates etc.
* deploy_example.yml is used to create a deployment object.

