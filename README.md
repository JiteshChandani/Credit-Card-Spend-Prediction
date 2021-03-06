# Predicting Credit Card Spend

# Business Problem:

One of the global banks would like to understand what factors driving credit card spend are. The 
bank want use these insights to calculate credit limit. In order to solve the problem, the bank 
conducted survey of 5000 customers and collected data. 
The objective of this case study is to understand what's driving the total spend (Primary Card + 
Secondary card). Given the factors, predict credit limit for the new applicants

Steps followed in deploying Machine Learning model using flask to Heroku are-

# 1. Train ML model

We have used Linear regression, Decision Tree, Random Forest and KNN algorithms however have used Random Forest technique to get the Machine Learning model in predicting the credit card spend.

# 2. Create a web app using Flask

I have defined the app routes and completing the main.py file, and created a index.html which will serve as the home page, which contains all the field required to run the model.

![pocoo_flask_logo_icon_168045](https://user-images.githubusercontent.com/75501488/138834924-7171e1a9-e449-4b31-98e2-e55a63794f35.png)


# 3. Commit the code to GitHub

Now create some of the required files for deployement and then commit all the files to GitHub.

Most important thing is to create a Procfile and requirement.txt, which handles the configuration part in order to deploy the model into heroku server. 
web: gunicorn is the fixed command, after that the first parameter is main.py file i.e the file which will be executed first. Provide the first parameter without the file extension. 
Second parameter is the flask app name. Requirements consists of all the libraries that has to get installed in heroku environment.

# 4. Connect GitHub to Heroku

Heroku is a multi-language cloud application platform that enables developers to deploy, scale, and manage their applications. Heroku is elegant, flexible, and easy to use, offering developers the simplest path to getting their apps to market.
Heroku gives the direct option to connect with GitHub and deploy the code.

![image](https://user-images.githubusercontent.com/75501488/138836204-bdfc04d7-1a20-494f-b5d7-23fa5ef70999.png)

# 5. Deploy the model

After successful deployment, app will be created. Check out the web-app: https://credit-card-spend.herokuapp.com/
