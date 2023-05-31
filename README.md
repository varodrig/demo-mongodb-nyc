# Demo for MongoDB .local NYC # 


##  Lab Instructions

Pre-reqs:

Check requirements: https://www.mongodb.com/docs/atlas/getting-started
Follow create an account: https://www.mongodb.com/docs/atlas/tutorial/create-atlas-account/
Follow Add your IP Address to your account to ensure your OpenShift cluster will have connectivity with Atlas: https://www.mongodb.com/docs/atlas/security/add-ip-address-to-list/


1. Install the operator
1. Create a project for the application
	oc new-project demo
2. Create the OpenShift manifests to deploy the application Quarkus super Heroes
	oc apply -f app-deploy/java17-openshift.yml

* Additional documentation about Quarkus Super Heroes https://github.com/quarkusio/quarkus-super-heroes
3. Validate all the pods are running on the namespace. $ oc get pods -w
4. Access the frontend application: UI Super Heroes.
	$ oc get routes -n demo 
* Test the UI Super Heroes to ensure it is working as expected.
* Follow the instruction on the Article MongoDB Atlas. Use this files as guide.

### Update the rest fights application to connect to the new database.
* oc apply -f oc apply -f app-deploy/rest-fights-new.yml



