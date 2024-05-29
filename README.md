# ARQe ( Augmented Reality based Quality Education )  

ARQe mainly focuses that lets educators and students create their own AR experiences by placing 3D models on reality.  It is not specific to any subject or grade, and can be used throughout various disciplines.  Additionally, Through NLP integrated model the Question bot finds solutions to the creative thinker’s questions. Our app has various applied concepts of different fields and current updates. Normal, Android users can access the AR models created with the featured specs of mobile. As result, while visualising the models they can be captured or recorded too.

## Authentication Screen:
This screen contains Login and Register Buttons which take you to their respective screens. 
The Login Screen has two text fields Mail Id and Password, a Login button which checks the Firebase backend data for a registered user and redirects to the Home screen and a Forgot Password button which takes you to a new screen where you need to enter your mail id to receive a link to reset your password.
The Register Screen has two text fields Mail Id and Password and a Register Button which creates a new entry in the Firebase authentication (FireAuth) and sends an verification mail to your account to confirm the entry.

## Home Screen:
This screen contains tiles of different topics with a Question Bot icon on the bottom right.
Each topic tile consists of the information about that respective model and a Model View button at the bottom right which redirects to the 3D model page with a AR View button at the bottom right corner.
The Model View Button loads the 3D model from Flask API backend and displays it
The AR View Button opens the Google AR core module in the device and projects the digital visual elements of the respective model, which can also capture and record the projected model.

## NLP Question Bot:
It is a pretrained model has two parameters context and questions. Context consists of information about the topics and the Question consists of questions based on the context. Context is a static data and Question will be sent as html form to the Model through flask api and the result will be sent from the api to display in the in the Question bot screen.
