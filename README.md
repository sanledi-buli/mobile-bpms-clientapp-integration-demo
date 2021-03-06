Red Hat Mobile Application Platform & JBoss BPMSuite Integration Client App Demo
================================================================================

This is the Red Hat Mobile Application Platform (MAP) - JBoss BPMSuite (BPMS) integration demo that provides examples of a form-based client application (Cordova Light Forms App).

Import the project into RH MAP
------------------------------
* Prerequisites:
	- Obtain a login and domain from the Red Hat Mobile team if you don't already have them.
	- You have already created a Bare Project and imported the [Cloud App](https://github.com/jbossdemocentral/mobile-bpms-cloudapp-integration-demo)

1. Login to the appropriate RH MAP domain.

2. Create a Client App ('+' to the top-right corner of Apps) -> Import Existing App -> Cordova Light -> Next -> Enter App Name -> select Public Git Repository

3. Enter Git URL as https://github.com/jbossdemocentral/mobile-bpms-clientapp-integration-demo.git -> Import and move onto integration

4. Download the form from github gist - https://gist.github.com/hucmaggie/b0a7382d9d6ea49559d7

5. Import the form file by using the RHMAP command line interface:
        `fhc appforms forms create --formfile=RHSummit2015AutoClaimFormsApp.json`

6. The original theme used in the demo is available as a github gist as well if you want to use it - https://gist.github.com/hucmaggie/72c461a2b9d5ac54a7e5

7. Import the themes file by using the RHMAP command line interface:
        `fhc appforms themes create --themefile=MaggiesSummit2015Theme.json`

8. Associate the form and theme with your project by going to Projects -> select your project -> Client App -> Forms -> select the imported theme & form -> Save. ![alt text](https://raw.githubusercontent.com/jbossdemocentral/mobile-bpms-clientapp-integration-demo/master/screenshots/RHMAP%20FormAndTheme.png "RHMAP Form + Theme")  

9. Rebuild the Client App (left panel of the client app). ![alt text](https://raw.githubusercontent.com/jbossdemocentral/mobile-bpms-clientapp-integration-demo/master/screenshots/RHMAPClientAppBuild.png "RHMAP Client App Build")

Notes
-----
This project is a bare git repo for the client app that can be imported into RH MAP.
The form and theme would need to be imported manually using fhc.

Supporting Articles
-------------------
- [Red Hat Mobile Application Platform - Connecting to JBoss BPMSuite REST (Special Edition for Red Hat Summit 2015!)](http://maggiechu-jboss.blogspot.com/2015/06/red-hat-mobile-app-connecting-to-bpms-rest.html)
- [Using the Red Hat Mobile Unified Push Server](http://www.ossmentor.com/2015/07/using-red-hat-mobile-unified-push-server.html)