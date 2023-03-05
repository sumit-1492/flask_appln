# flask_appln

### Implementation of simple flask application

'''
@app.route("/") 
'''
'''
@app.route("/sumit") 
'''
Docker implementated

### first step - docker image should be created
'''
docker build -t sumit .
'''
### second step - we have to give port number in our app.py file
'''
app.run(host = '0.0.0.0',port = 8000)
'''
'''
doker run -d -p 8000:8000 sumit
'''
### if you want to stop any docker container of any docker image
'''
dcoker ps
'''
### 
'''
docker stop <container id>
'''

## @app.route("/") - we do not give any route to our apllication we will reach on local host only
## @app.route("/sumit") - here we have route called sumit so in local host we to provide sumit
## docker build -t sumit .  - building a docker image named sumit, . means current directory
## doker run -d -p 8000:8000 sumit - d - detach, p - port , sumit - docker image name
## dcoker ps - it will show status of docker image and its container
## docker stop <container id> - it will stop the container id of the docker image running
