# flask_appln

Implementation of simple flask application

'''
@app.route("/") 
@app.route("/sumit") 
'''
1. @app.route("/") ## we do not give any route to our apllication we will reach on local host only
2. @app.route("/sumit") ## here we have route called sumit so in local host we to provide sumit

Docker implementated
## first step - docker image should be created
'''
docker build -t sumit .
'''
3. docker build -t sumit . ## building a docker image named sumit, . means current directory
## second step - we have to give port number in our app.py file
'''
app.run(host = '0.0.0.0',port = 8000)
'''
'''
doker run -d -p 8000:8000 sumit
'''
4. doker run -d -p 8000:8000 sumit ## d - detach, p - port , sumit - docker image name

## if you want to stop any docker container of any docker image
'''
dcoker ps
'''
5. dcoker ps ## it will show status of docker image and its container

'''
docker stop <container id>
'''
6. docker stop <container id> ## it will stop the container id of the docker image running
