# Demo NodeJS with Gitlab CI and Heroku

A simple example of integration of NodeJS application with Gitlab CI and Heroku delivery.

## How it works

1. Clone the project and deploy as Gitlab repository. 
2. Create an app on Heroku. 
3. Using for example `heroku-cli` make sure you made an initial commit (push) to Heroku repository manually, otherwise you may get an error in Gitlab CI pipeline step.
4. Set the environmental variables for your Gitlab repository:

- `HEROKU_API_KEY` : your API key taken from Heroku (under your profile settings)
- `HEROKU_REPO_NAME` : name of your Heroku repository, also the abbreviation of your web app project name in Heroku
- `BASE_LIVE_URL` : URL to your Heroku environment (full URL including https://)

5. Push your code, go to Gitlab CI/CD and press a button to deploy to Heroku. 
