# Shopping List Frontend For Practicing Deployment

When deploying the front end:

- Make sure you set the `REACT_APP_BACKEND_URL` environment variable (because at build time, the build process will take the values available and inject/hard code them into the generated files).
- Have a look at the typical build settings (for a typical project folder structure): https://docs.netlify.com/configure-builds/common-configurations/#create-react-app


## DEPLOYING HEROKU TO THE BACKEND VIA THE COMMAND LINE

1. brew tap heroku/brew && brew install heroku
    - installs heroku

2. heroku login
    - you need to login here to continue successfully
    
3. heroku git:remote -a "shopping-backend-leo-hassan"
    - accesses the the heroku database(app)

4. git add .
5. git commit -am "initial commit"
6. git push heroku master
    - these are the add, commit, push commands when using heroku

7. heroku open
    - opens backend web page with URL. This URL is used for the .env file in the frontend