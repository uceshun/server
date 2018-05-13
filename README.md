Technical Report
There is a purpose to set up three components in this project to keep the location-based quiz run and serve the users. They are the the AppServer, QuestionsApp and the QuizApp. The database server is supported by postgreSQL/PGAdmin4.

NodeJS Server: AppServer
The AppServer repository, as a web server, receive request from web and mobile, also reponse back to them, as well as storing data in both the web and mobile applications. A HTTP server is used for both the QuizApp and QuestionsApp.In the code, GET and POST commands are used to download and upload data in both the QuizApp and QuestionsApp

Installation Guide (Guide from practical notes)
1. In terminal type: git clone https://github.com/uceshun/server, to clone the AppServer repository
2. Go to the AppServer directory using the terminal: "~/code/AppServer"
3. Run the server in the background, by typing "node httpServer.js &".
4. Bring the server back to the foreground so that you can stop it by typing: "fg 1" which will display the current running servers 
5. Stoping the server, typing :"Ctrl+C".

Now you have running the httpServer.js in the background

Technical Information
HTTP: 30298
HTTPS: 31098
Phonegap: 31298


Web Application: Questions Setting App
This application is aimed to create the questioners and correct answers, by clicking the point on a Leaflet map, which are saved in to database on the web server.


Installation Guide
1. In terminal type: git clone https://github.com/uceshun/QuestionsApp, to clone the Question Setting repository
2. Now please make sure the Appserver have running by following installaion guide earlier
3. Go to the QuestionsApp directory and run the phonegap server: "~/code/QuestionsApp/uceshun" and enter "phonegap serve"


Mobile Application: QuizApp
This application is aimed to collect end-users’ answer data from quiz and save to database. The application can monitor the end-users’ movement and guide them by the map (, which will be explained in next session), and lead them to answer pop-up questions, as well as providing user the correct answer, which are set by Question Setting Application.


Installation Guide
1. In terminal type: git clone https://github.com/uceshun/quiz, to clone the Question Setting repository
2. Now please make sure the Appserver have running by following installaion guide earlier
3. Go to the QuestionsApp directory and run the phonegap server: "~/code/quiz/uceshun" and enter "phonegap serve"


At the end, all my works are accredited to Claire and my classmates, they guide and lead me a lot while i was lost :)
Code adapted from: https://github.com/claireellul/cegeg077-week5server/blob/master/httpServer.js
Code adapted from: https://github.com/claireellul/cegeg077-week5app/blob/master/ucfscde/www/js/appActivity.js
Code adapted from: https://github.com/claireellul/cegeg077-week6formcode
