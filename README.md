# Node.js Redis Cache Web Starter Overview

This is a port of the [Node.js Cache Web Starter](https://github.com/IBM-Bluemix/nodejs-datacache)  that demonstrates how to use the Bluemix Data Cache service. 

This  uses  the Bluemix Community Redis  service instead because Community Redis has a free plan and the Bluemix Data Cache does not have one anymore. 
Other than using Redis instead of the Bluemix Data Cache Service as the back end for storing data, this app is the same as the  Node.js Cache Web Starter. It lets the user enter key-value pairs to cache, then looks up or deletes keys and changes existing cached values.

If deploying to Bluemix, note that the Redis  service is a community service from Cloud Foundry and is listed as *Experimental*. 

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy)

## Run the app locally

This app will run locally using an in-memory cache instead of the Redis service if the VCAP_SERVICES environment variable is not set.

1. [Install Node.js][]
2. Download and extract the starter code from the Bluemix UI
3. cd into the app directory
4. Run `npm install` to install the app's dependencies
5. Run `npm start` to start the app
6. Access the running app in a browser at http://localhost:3000

[Install Node.js]: https://nodejs.org/en/download/

# Privacy Notice
Sample web applications that include this tracking library may be configured to track deployments to [IBM Bluemix](https://www.bluemix.net/) and other Cloud Foundry platforms. The following information is sent to a [Deployment Tracker](https://github.com/IBM-Bluemix/cf-deployment-tracker-service) service on each deployment by default:
* Application Name (`application_name`)
* Space ID (`space_id`)
* Application Version (`application_version`)
* Application URIs (`application_uris`)

This data is collected from the `VCAP_APPLICATION` environment variable in IBM Bluemix and other Cloud Foundry platforms. This data is used by IBM to track metrics around deployments of sample applications to IBM Bluemix to measure the usefulness of our examples, so that we can continuously improve the content we offer to you. 
