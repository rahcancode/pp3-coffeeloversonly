## OVERVIEW
I wanted to create a very simple database so that a small coffee shop owner could tally the types of coffee they sold every day.

The fully deployed project can be accessed here: https://coffee-lovers-only.herokuapp.com/ 

![Responsive Image](https://github.com/rahcancode/pp3-coffeeloversonly/blob/main/media/responsive.JPG)

## UX/UI
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

## DESIGN/FEATURES

- Design is simple, with an coffee cup and project title depicted in ascii art
- Instructions on what coffees are sold and how to input the data is clearly listed
- Humorous actions are noted while the data is being calculated and updated, taking inspiration from [The Sims "Reticulating splines"](https://sims.fandom.com/wiki/Reticulating_splines).

- Main terminal image
![Main terminal image](https://github.com/rahcancode/pp3-coffeeloversonly/blob/main/media/mainterminal.JPG)

- A validation error appears when too many or not enough numbers are entered
![Validation error](https://github.com/rahcancode/pp3-coffeeloversonly/blob/main/media/validationerror1.JPG)

- A string of validation confirmation messages are listed when data is input correctly, and an exit message is shown
![Validation confirmation and exit message](https://github.com/rahcancode/pp3-coffeeloversonly/blob/main/media/validationconfirmed.JPG)


FUTURE FEATURES
- Separate the inputs for each individual coffee (i.e "Number of Americanos sold: X, Number of Flat Whites sold: Y, etc)
- Tally the amount of coffee needed, used and wasted based on sales, surplus and stock calculations

BUGS OR ERRORS
- No bugs or errors found

## TESTING
- As the program is quite basic, testing was simple
- `<valiate_data()>` is used to ensure there are six numbers entered and validated against the `<sales_data>`
- A `<ValueError>` is raised when either not enough or too many numbers are entered
- A `<ValueError>` is raised when letters or words are entered instead of numbers
- The code passed through the PEP8 linter with no errors

MODULES IMPORTED
- `<google.oauth2.service_account>` for using the Credentials function on `<creds.json>` file
- This was used to link the program with [the Google spreadsheet](https://docs.google.com/spreadsheets/d/1XQeltrBNdDc4yRPAbMRcgY_NmDyEeVGKUQgkfR8WkrM/edit?usp=sharing) using the `<gspread>` module

## DEPLOYMENT
The project was deployed using a mock terminal from Code Institute, by way of Heroku.

Steps to deploy:
- Fork or clone [the template from Code Institute for Project 3](https://github.com/Code-Institute-Org/p3-template)
- Create a new Heroku app
- Set Buildpacks to `<heroku/python>` and `<heroku/nodejs>` in that order
- Reveal Config Vars, and copy/paste data from `<creds.json>` file to key and value respectively
- Add in another Config Var of key: Port and value: 8000
- Link Heroku app to the repository
- Hit deploy!

## CREDITS
The video run through's for the Love Sandwiches project were used as key reference points when building the outline of the program.

[asciiart.eu](asciiart.eu) - for the coffee mug ascii art

[learnlearn.uk](learnlearn.uk/python/ascii-art/) - for how to add the ascii art to my project

[patorjk.com](patorjk.com/software/taag/#p=testall&f=Efti%20Wall&t=Coffee%20Lovers%20Only) - for the ascii text of "Coffee Lovers Only", in font Efti Wall

## TOOLS
[GitHub](https://github.com/) - used for hosting the source code of the program
[Gitpod](https://www.gitpod.io/) - used for testing the program
[PEP8 Validator](https://pep8ci.herokuapp.com/#) - used for validating the python code
[Heroku](https://www.heroku.com/home) - used for deploying the project
