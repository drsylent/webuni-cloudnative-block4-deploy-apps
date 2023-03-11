# webuni-cloudnative-block4-deploy-apps
WebUni Cloud-Native Application Development training's 4th block - application deployment configuration

# How to start the api application
helm upgrade api spring-webuni --install -f api.yaml -n webuni

# How to start the db application
helm upgrade db spring-webuni --install -f db.yaml -n webuni --set env[2].value=<ENTER-PASSWORD>
