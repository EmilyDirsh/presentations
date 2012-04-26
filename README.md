My OpenShift PaaS Presentations
==================================

These are a collection of presentations that
I've given during my time working on OpenShift.

Running this on OpenShift
==================================

Create an account at http://openshift.redhat.com/

Create a ruby-1.8 application

    rhc app create -a showoff -t ruby-1.8

Then add this repo

    cd showoff 
    git remote add upstream -m master git://github.com/matthicksj/presentations.git
    git pull -s recursive -X theirs upstream master

Add your showoff files
    
Then push the repo upstream

    git push

You can now view these presentation at:

    http://showoff-$yournamespace.rhcloud.com

Customize away!
