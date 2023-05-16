# Final-Project-Assessment-for-Scalefocus-Academy

The Final Project for academy 2023 - Deploy a WordPress on Kubernetes (using Minicube) with Helm and
automation with Jenkins

To start the project we need to have Kubernetes, Helm and Jenkins installed
Clone the bitnami chart for github repository
https://github.com/bitnami/charts/tree/main/bitnami/wordpress

In the values.yaml file we are changing line 534 from Loadbalancer to clusterIP
Loadbalancer to cluster IP.jpg
