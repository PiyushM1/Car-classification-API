# Car-classification-API

The API was developed using Flask. It loads 3 models that I trained [here](https://github.com/PiyushM1/Car-make-model-and-year-classifier) using [Monk library](https://github.com/Tessellate-Imaging/monk_v1), receives pictures from the user and returns the predicted make, model and year.

### Setup
- Clone this repository, or download as zip and extract to a directory
- Activate the virtual environment
- Install the requirements using `pip install -r requirements.txt`

### Usage
- Run the app using `python app.py`
- To test the API using cURL
  - Install cURL using `pip install curl`
  - Run the following command after updating the path to the image 
  
    `curl -X POST -F file=@<image_path> 'http://0.0.0.0:5000/predict'`
- To test the API using a user interface
  - Open http://0.0.0.0:5000 in a web browser
  - Upload an image using the webpage and press the predict button
