# Final-Project-Assessment-for-Scalefocus-Academy


Deploy a WordPress on Kubernetes (using Minicube) with Helm and automation with Jenkins

To start the project we need to have Kubernetes, Helm and Jenkins installed on out machine and we need to create new github repository bu the name Final Project Assessment for Scalefocus Academy


Download Helm chart for WordPress
https://github.com/bitnami/charts/tree/main/bitnami/wordpress



And change the values.yaml - line 534 from Loadbalancer to clusterIP
![image](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/d735bd29-30cb-4a47-a8f7-eb093f65b323)



Start the kubernetes claster using minikube 
check if the pods/nodes are running 
![Get pods, nodes ](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/7a07907e-7b12-4fad-aca8-744c5e1a6e20)



Install Kubernetes plugins and Create Jenkins Pipeline
Jenkinsfile will be needed as well to help us create the Jenkins pipeline that checks if wp namespace exists, if it doesn’t then it creates one.
also will check if WordPress exists, if it doesn’t then it installs the chart.
![Jenkind pipeline](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/d028da4b-2791-49aa-8639-0db3e140e03b)




name the Helm Deployment as: final-project-wp-scalefocus
![Helm  final-project-wp-scalefocus ](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/379881cd-f8ac-4249-9682-d9ae55077631)



forward the port to open in localhost
![port forward to localhost](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/0fb9bb48-67f3-4b07-a045-738cd62cbd9c)
 
 
 
 open the wordpress in the browser 
 Load the home page of the WordPress to see the final result. 

 ![page wordpress](https://github.com/monikakostovska/Final-Project-Assessment-for-Scalefocus-Academy/assets/85322121/eb4a9ac8-3ae0-40b6-8bd4-5b844d13752d)
