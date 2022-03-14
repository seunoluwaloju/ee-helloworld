

## Local Development
### Pre-requisites
1. Install python3
2. Install virualenv

### Setup virtual environment
```shell
python3 -m pip install --user virtualenv
```
3. Create virtual environment
```shell
python3 -m venv venv
```
4. Activate virtual environment
```shell
source venv/bin/activate
```
5. Install required libraries
```shell
pip3 install -r requirements.txt
```
### Run web app locally
1. With virtual environment being activated, run the following command
```shell
python3 app.py
```
2. Go to http://127.0.0.1:5000 and verify you see `Hello Equal Experts`

### Run tests
To execute test for the project, from the project root directory, run the following command
```shell
pytest 
```

### Build and run docker image locally
1. To build the docker image, while under the root directory, run the following command
```shell
docker build -t helloworld .
```
2. Run the docker container with the following command
```shell
docker run -d -p 5000:5000 helloworld
```
3. Go to http://127.0.0.1:5000 and verify you see `Hello Equal Experts`