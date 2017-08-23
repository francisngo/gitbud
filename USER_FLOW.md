## Login/Signup

- The landing page is the entry point to the app. 
- Handled by the Landing react component, the user has the option to login with Github. 
- Clicking the login button will send a GET request to the url /auth/github.
- If this is the user's first time, the user will be routed to the Questionnaire component.
  - This logic is handled App component, where a check is made to see if the user's loggedIn state has certain properties.
- If the user has logged in before, then they will be redirected to a project list page.

## Questionniare

- This page asks the user for:
    - Experience Level
    - Interested Language
    - Profile Descripion
- This info is stored in the user's node in the database and is displayed in the user's profile.
- After completing the questionnaire, user is taken to the Project List page.

## Project List
- This can be considered the home page.
- The list of available projects to work on will be displated
- Clicking on a project will have 2 possibe outcomes:
    - If the user is not working on the project, they will be taken to the project details page.
    - If the user is already working on the project with a pair, they will be taken to the Project Status page.
- This logic is handled inside a 'smart' Project container.
- The container checks the user's state to see whether the user is paired on a project or not, and renders the appropriate component.

## Project Details


## User List

## User Details

## Project Status

## My Projects

## My Account