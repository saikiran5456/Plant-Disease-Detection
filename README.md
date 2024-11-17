# Plant-Disease-Detection

An Artificial Intelligence and Cloud Based Collaborative Platform for Plant Disease Identification, Tracking and Forecasting for Farmers

In this project author using convolution neural networks as artificial intelligence to train all plant diseases images and then upon uploading new images CNN will predict plant disease available in uploaded image. For storing CNN train model and images author is using cloud services. So using AI author predicting plant disease and cloud is used to store data.

In this project author using smart phone to upload image but designing android application will take extra cost and time so we build it as PYTHON web application. Using this web application CNN model will get trained and user can upload images and then application will apply CNN model on uploaded image to predict disease. If this web application deployed on real web server then it will extract user’s location from request object and can display those locations in map. If you run in local machine then we will get default IP ‘127.0.0.1’ and for this IP will get only default latitude and longitude. 

To implement this project we are using plant disease images dataset from ‘PlantVillage’ web site.

Python Django Server act like a cloud and web server

MYSQL database: used to store user’s details and their uploaded images location details.

To run this project install python 3.7 and then install MYSQL database and create database in MYSQL by copying content from ‘DB.txt’ file and paste in MYSQL.

Install below packages by opening command prompt and executing below commands

Pip install django
Pip install pymysql
pip install geoip2

after installing above command put ‘PlantDisease’ folder in any directory of your system and then open command prompt and set location to PlantDisease and execute below command to start server

python manage.py runserver

after executing above command will get below server screen

![image](https://github.com/user-attachments/assets/a6c7eb05-0438-4ec1-bbc5-aea440a6bbd4)

 
In above screen python server started and running on IP http://127.0.0.1:8000’. Now open browser and enter URL as ‘http://127.0.0.1:8000/index.html’ to get below screen

 ![image](https://github.com/user-attachments/assets/117ca671-4338-4ad4-bd10-cdedc10ae156)


In above screen click on ‘Register Here’ link to allow user to register with the application

![image](https://github.com/user-attachments/assets/32aaf993-6731-44b4-a816-b5b40f4eb555)

 
In above screen click on ‘Register’ button to add new user

![image](https://github.com/user-attachments/assets/53c33102-df1b-4fe0-ac55-d42af337bbc7)

 
In above screen user signup process completed. Now user can click on ‘Login’ link to login to application

 ![image](https://github.com/user-attachments/assets/9e1bd20b-1eb6-4a30-bf5a-a526a5f897ad)

After login will get below screen

![image](https://github.com/user-attachments/assets/6ac70a11-da53-4c78-b353-34e398bbf91b)

 
In above screen click on ‘Upload Plant Image’ link to get below screen

![image](https://github.com/user-attachments/assets/c83d4377-e36e-4d56-a9e3-ab2b67d21074)

 
In above screen user can upload image of his crop to predict disease using CNN

![image](https://github.com/user-attachments/assets/e956136c-2a37-4373-88f6-fcc9849b5454)

 
In above screen uploading 1.JPG image and now click on ‘Open’ button to upload image

![image](https://github.com/user-attachments/assets/53399a7e-2e76-4065-84a8-6f94eedd9e30)

 
In above screen click on ‘Submit’ button to predict disease

![image](https://github.com/user-attachments/assets/0fddc1fa-de2f-4b68-b5c7-9caf66c4710a)

 
In above screen we will get image with predicted disease name printed on image and now close that image to get locations in map

 ![image](https://github.com/user-attachments/assets/f754515f-9f74-4e4a-b3e0-21284f3d2c8f)

In above screen in map we can get location of uploaded image mark with marker and below map we can see predicted disease name in red colour. Similarly you can upload any image from ‘uploadimages’ folder. In below screen we can see CNN layers created to build plant disease model

 ![image](https://github.com/user-attachments/assets/4b2ef86e-9413-4a92-9b8b-8885a50f2662)

In above screen we can see CNN multi layers filter created where first filter created with image size 62 X 62 and second filter with size 31 X 31 and goes on.
