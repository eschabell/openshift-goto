Red Hat Developer Day London mobile registration app on OpenShift
=================================================================

This is the Red Hat Developer Day London 2012 html5/mboile registration app.

Running on OpenShift
--------------------

Create an account at http://openshift.redhat.com/

Create a jbosseap-6.0 application

    rhc app create -a devdayuk -t jbosseap-6.0

Add this upstream cloudtour repo

    cd devdayuk
    git remote add upstream -m master git://github.com/eschabell/openshift-devdayuk.git
    git pull -s recursive -X theirs upstream master

Then push the repo upstream

    git push

That's it, you can now checkout your application at:

    http://devdayuk-$namespace.rhcloud.com

Don't forget it is better in your mobile browsers!
