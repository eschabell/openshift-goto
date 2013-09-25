GOTO 2013 mobile registration app on OpenShift
==============================================

This is the GOTO 2013 html5/mboile registration app.

Running on OpenShift
--------------------

Create an account at http://openshift.redhat.com/

Create a jbosseap-6.0 application

    rhc app create -a devdayuk -t jbosseap-6.0 --from-code git://github.com/eschabell/openshift-goto.git

That's it, you can now checkout your application at:

    http://goto-$namespace.rhcloud.com

Don't forget it is better in your mobile browsers!
