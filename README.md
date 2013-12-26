JBoss Business Optimizer Demo 
=============================

Explore the running demo on OpenShift.

Create an account at http://openshift.redhat.com

Create a JBoss EAP 6 application

    rhc app create optimizer -t jbosseap-6

Add this upstream openshift-businesss-resource-optimizer repository

    cd optimizer
    
    git remote add upstream -m master git://github.com/eschabell/openshift-business-resource-optimizer.git
 
    git pull -s recursive -X theirs upstream master

Then push the repo upstream

    git push

That's it, you can now checkout your application at:

    http://optimizer-$your_domain.rhcloud.com/optaplanner-webexamples-6.0.0-redhat-6


QuickStart Screenshots
----------------------

![Cloud Balancing] (https://github.com/eschabell/business-resource-planner-demo/blob/master/docs/demo-images/cloud-balancing.png?raw=true)

![Vehicle Routing] (https://github.com/eschabell/business-resource-planner-demo/blob/master/docs/demo-images/vehicle-routing.png?raw=true)
