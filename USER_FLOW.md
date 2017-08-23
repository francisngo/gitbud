#GitBud User Flow

##Login/Signup

- The landing page is the entry point to the app. 
- Handled by the Landing react component, the user has the option to login with Github. 
- Clicking the login button will send a GET request to the url /auth/github.
- If this is the user's first time, the user will be routed to the Questionnaire component.
  - This logic is handled App component, where a check is made to see if the user's loggedIn state has certain properties.
- If the user has logged in before, then they will be redirected to a project list page.

##Questionniare

- This page asks the user for:
  - Experience Level
  - Interested Language
  - Profile Descripion
- This info is stored in the user's node in the database and is displayed in the user's profile.
- After completing the questionnaire, user is taken to the Project List page.

##Project List

##Project Details

##User List

##User Details

##Project Status

##My Projects

##My Account