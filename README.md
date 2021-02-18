# Dating_App_1

ML model can be integrated using Flask Framework and Flutter App. Rest API is created using Flask framework and requests are sent to it via Flutter App.
WEBSCRAPING – 
Web Scraping is used to create columns like User Biography, Gender, and Age, Ratings for Movies, TV, Religion, Music, Sports, Books, and Politics. 
CREATING THE MODEL - 
Standardization is used here so that all features except biography column can get the same weightage. Here using Standardization we can get mean of 0 and standard deviation of 1. Then the biography column is extracted from the data frame and NLP is used here to remove stop words, introduce stemming and then converted into array of words. This array is combined with the standardized data. Then the model is trained using K Means Clustering Algorithm. KMeans clustering is used here to train the model and cluster them. The model and column names will be available to the flask server using pickling.
CREATING THE FLASK SERVER – 
The POST requests from the flutter app will be sent to the “/predict” route. The model and the column names are fetched and used for prediction. User Biography along with Age and Gender will be returned in the JSON format. In the future, User_Name and User_Profile_Photo Columns also should be added, so that it returns User_Name and User_Profile_Photo. And when the user clicks on the output it should show other details like Biography, Age, Gender, etc.
DEPLOYING THE API – 
In order to use the API, it is deployed using Heroku.
FLUTTER APP –
The parameters for the model mentioned above are taken as input from the user via text fields. The HTTP package is used to make post requests to the server.

 

