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

6. Note that Heroku should automatically choose "Node JS" buildpack.

7. Once the deployment is complete (check Heroku logs too, not only Gitlab) application should restart and start. Visit the main URL to see 'Hello World!' text.

## How to start

Heroku launches `npm start` automatically in a free mode, once the package is deployed. You can run this command to execute a simple Express server with 'Hello World!' text.