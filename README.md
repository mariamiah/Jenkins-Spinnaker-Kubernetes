### Jenkins-Spinnaker-Kubernetes
The purpose of this project is to create a reliable and robust continuous delivery pipeline using Google Container Engine (GKE), Google Cloud Source Repositories (GSR), Google Cloud Container Builder (GCB), and Spinnaker. You deploy your code changes in an automated fashion with the ability to quickly roll back your deployments. 

Using a sample application, a configuration of the above services is done to automatically build, test and deploy the application.
If any change is made to the application, the continous delivery pipeline is triggered to automatically rebuild, test and redeploy the new version.

The project comprises of a set of terraform files designed to create a cloud environment from scratch using Jenkins and Spinnaker

### Spinnaker
- This provides application management and application deployment services.
#### Application management
- With application management, one is able to view and manage cloud resources
#### Key concepts used by  spinnaker
(To describe services)
- Applications - The collection of clusters. It includes firewalls and load balancers. An application represents the service which needs to be deployed using spinnaker, configuration for the service, infrastructure on which it will run
- Clusters - The collection of server groups irrespective of any kubernetes clusters that may exist in the underlying architecture.(This doesnot map to the kubernetes cluster)
- Server groups
(To describe how services are exposed to users)
- Load balancers - This is associated with the ingress protocol and port range. It balances traffic among instances in its server groups
- Firewalls - This defines the network traffic access. It is a set of firewall rules defined by IP range(CIDR) along with a communication protocol TCP and port range
#### Application deployment


