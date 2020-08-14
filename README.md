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
$ functions-framework --target handler --debug
$ curl -v http://0.0.0.0:8080/
```

