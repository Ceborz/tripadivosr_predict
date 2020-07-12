## Project setup
Install conda
Create enviroment for conda
In the enviroment run
```
conda install python
conda install -c anaconda pandas
conda install -c conda-forge matplotlib
pip install -r requirements.txt
```
## Run API
```
uvicorn api.main:app --reload
```
This will run a local server on http://127.0.0.1
## Run training
Call a post with the api running to http://127.0.0.1/train
## Test predictions
Call a get with the api running to http://127.0.0.1/predict
This request receives a query param "sentences" that is an array of sentences to predict