# Dependencies

* express
* hbs
* wax-on
* handlebars-helpers
* mongodb
* dotenv


# Setup 

1. Create .env file with MONGO_URL 

2. yarn install (since repo is forked)

3. Login to Heroku in terminal (email & pwd)

4. To create a deployment to Heroku:
in terminal: heroku create <unique file name>

5. In terminal: git remote -v 

6. Create Procfile (same directory as index.js)
```web: node index.js``` into Procfile 
6.1 Save Procfile
**Heroku looks for this file for it to run**

7. In package.json, under scripts include 
```"start":"node index.js"```

8. Change the 3000 in port to ```process.env.PORT```

### Ensure all project is working fine before deploying to Heroku
Easier to debug in Dev env than debugging in Heroku

### When deploying to Heroku: 
1. ```git add .```
2. ```git commit -m "<your commit messages>"```
3. ```git push heroku```



1st method: 
go to react folder
npm run build 
this will create a build folder in the project file 
right-clicked build and download the build folder
unzipped the build folder (using 7zip)
extract to the folder
in netlify, under Sites 
drag the extracted folder into Sites


2nd method:
react app must be in the root folder
select new site from Git (from netlify)
search react repository 
