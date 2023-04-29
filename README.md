## OVERVIEW
I wanted to create a very simple database so that a small coffee shop owner could tally the types of coffee they sold every day.

The fully deployed project can be accessed here: https://coffee-lovers-only.herokuapp.com/

~SCREENSHOT~

UX/UI
STRATEGY
Goals
- Simple command line input, so that anyone with any level of computer knowledge could easily enter data
- The program should access the right worksheets in Google Sheets: sales, surplus and stock
- The program should calculate the surplus worksheet correctly based on the sales and stock levels
- The program should update the surplus worksheet sheet with the right values

SCOPE
- The user's data input will be written on the screen
- The program displays warnings when the input of the user is not valid (i.e more/less values are input, letters/words are used instead of numbers)

STRUCTURE
- The terminal was created using the Code Institute template
- The program was coded with Python only
- Heroku is used to run the program

DESIGN/FEATURES

- Design is simple, with an coffee cup and project title depicted in ascii art
- Instructions on what coffees are sold and how to input the data is clearly listed
- Humourous actions are noted while the data is being caluclated and updated, taking inspiration from The Sims "Reticulating splines".


FUTURE FEATURES
- Separate the inputs for each individual coffee (i.e "Number of Americanos sold: X, Number of Flat Whites sold: Y, etc)
- Tally the amount of coffee needed, used and wasted based on sales, surplus and stock calculations

BUGS OR ERRORS
- No bugs or errors found

TESTING
- As the program is quite basic, testing was simple
- valiate_data() is used to ensure there are six numbers entered and validated against the sales_data
- a ValueError is raised when either not enough or too many numbers are entered
- a ValueError is raised when letters or words are entered instead of numbers

MODULES IMPORTED
- google.oauth2.service_account for using the Credentials function on "creds.json" file
- This was used to link the program with the Google spreadsheet using the gspread module

DEPLOYMENT
CREATING THE WEBSITE
I have used the Code Institute Python Essentials Template for creating a terminal where my Python code will generate its output. The steps were as follows:

Click the Use this template button
A New Repository page will appear, write a Repository name and a short description and press Create repository from template
Press the green Gitpod button to create your project workspace and start developing your website

DEPLOYING ON HEROKU
After finishing developing the program I deployed it on Heroku following the instructions:

Create an account and login into Heroku website
Click "New -> Create new app" button
Insert your app's Name and Choose your region then click the "Create App" button
Into the Settings tab go to "Config vars" section and click "Reveal Config Vars"
Enter the PORT in the KEY section and 8000 for its value, then click "Add"
Go to "Buildpacks" section and click "Add buildpack"
Firstly add the Python buildpack then NodeJs
Into the Deploy tab go to "Deployment method" and select Github
After that go to "App connected to GitHub" and look for your GitHub repository name to link it
You can now choose to either manually or automatically deploy your app to Heroku.
With automatic deploys enabled, Heroku will build a new version of the app each time a change has been pushed to the repository
Manual deploys means your app will be updated only when you manually click to deploy it
When the deploying is finished, a link will be provided to you for accessing your app
ollowed by the copied URL
Your clone was created

CREDITS
The code for linking to the Google Spreadsheet and manipulating it was taken and adapted from the Code Institute Love Sandwiches tutorial

TOOLS
GitHub - used for hosting the source code of the program
Gitpod Dev Environment - used for testing the program
PEP8 Validator - used for validating the python code
Heroku - used for deploying the project
asciiart.eu - for the coffee mug ascii art
https://learnlearn.uk/python/ascii-art/ - for how to add the ascii art to my project
http://patorjk.com/software/taag/#p=testall&f=Efti%20Wall&t=Coffee%20Lovers%20Only - for the ascii text of "Coffee Lovers Only", in font Efti Wall

ACKNOWLEDGEMENTS
