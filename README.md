### first_app
* create_pods.yml creates a basic POD definition for a defined docker container. We use kubectl expose to view the application.
* loadbalancer.yml is a loadbalancer service which was used to integrate AWS elastic load balancer to our application.We can then use the DNS name created with ELB to point to our customized domain name using route 53.

