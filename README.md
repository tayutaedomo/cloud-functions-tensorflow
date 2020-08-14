# cloud-functions-tensorflow
Try tensorflow on Cloud Functions


## Setup
```
$ git clone git@github.com:tayutaedomo/cloud-functions-tensorflow.git
$ cd cloud-functions-tensorflow
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install --upgrade pip
$ pip install -r requirements.txt
```


## Local Development
```
$ cd cloud-functions-tensorflow
$ functions-framework --target tensorflow_handler --debug
$ curl -v http://0.0.0.0:8080/
```


## Cloud Functions
```
$ cd cloud-functions-tensorflow
$ gcloud functions deploy tensorflow_handler --runtime python37 --memory 512MB --trigger-http --allow-unauthenticated
$ gcloud functions call tensorflow_handler
```

