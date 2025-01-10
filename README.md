# Install docmost on openshift or kubernetes 

# Prereq

Go in manifest folder and edit the docmost.yqml deployment with your smtp configuration (will be used to allow other user to register). <YOUR_APP_SECRET> <YOUR_SMTP_USERNAME> <YOUR_EMAIL_ADDRESS>

#

```shell
oc apply \
-f docmost.yaml \
-f route.yaml \
-f service.yaml \
-f pvc.yaml
```