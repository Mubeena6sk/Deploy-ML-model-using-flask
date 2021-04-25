# Deploy-ML-model-using-flask
This is a demo project to elaborate how Machine Learning Models are deployed using Flask API

3##Prerequisites
You must have 'requirements.txt' installed.

###Project Structure
This project has four major parts :
- model.py : This contains code for our Machine Learning model to predict employee salaries absed on traingin data in 'dataset.csv' file.
- app.py : This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
- request.py : This uses requests module to call APIs already defined in app.py and dispalys the returned value.
- templates : This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.

###Running the project
Ensure that you are in the project home directory. Create the machine learning model by running below command -
> python model.py
> 
This would create a serialized version of our model into a file model.pkl

Run app.py using below command to start Flask API
> python app.py
> 
By default, flask will run on port 5000.

Navigate to URL http://localhost:5000
You should be able to view the homepage as below : alt text

Enter valid numerical values in all 3 input boxes and hit Predict.
