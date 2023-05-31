# Demo for MongoDB .local NYC # 

##  Lab Instructions

1. Create a project for the application
	oc new-project demo
2. Create the OpenShift manifests to deploy the application Quarkus super Heroes
	oc apply -f app-deploy/java17-openshift.yml

* Additional documentation about Quarkus Super Heroes https://github.com/quarkusio/quarkus-super-heroes
3. Validate all the pods are running on the namespace.
4. Access the frontend application: UI Super Heroes.
	$ oc get routes -n demo 
* Test the UI Super Heroes to ensure it is working as expected.


