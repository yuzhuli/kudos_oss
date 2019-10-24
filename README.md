# kudos_oss

### Setup venv
* Check python version: python --version
* Install virtual environment: python3 -m venv ~/Dropbox/code/kudos_oss/venv (path to virtual env directory). Running this command creates the target directory (creating any parent directories that don’t exist already) and places a pyvenv.cfg file in it with a home key pointing to the Python installation from which the command was run (a common name for the target directory is .venv). 
* Activate venv: source venv/bin/activate

### Python Rest api with MongoDB 
* Install pymongo. 
* touch docker-compose.yml
* Add content to docker-compose.yml
* run: dock-compose up
* Run rest api: FLASK_APP=$PWD/app/http/api/endpoints.py FLASK_ENV=development pipenv run python -m flask run --port 4433

### Create React client-side app
* Install yarn: sudo npm install -g yarn
* Install create-react-app: yarn global add create-react-app
* Create a React application and put it in web directory: create-react-app app
* Run the react app: 
```
cd app
npm start
```

### Libraries
* Go to target directory: cd kudos_oss/
* Install Flask: pip install -U Flask
* Install marshmallow library for python model schemas: pip install -U marshmallow
* Install pymongo for python RESTful api persistence with MongoDB: pip install pymongo
* Install pyjwt to take care of the validation: pip install PyJWT
* Install CORS to implement CORS on Rest api: pip install -U flask-cors
