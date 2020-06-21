## TechLogs
### UI for interacting with tech database
---


This app will provide an interface to interact and share tech logs and special notes.

Using **handlebars** as templating engine.

---
### Configuration

Added { "start": "cross-env NODE_ENV=production node app", "dev": "cross-env NODE_ENV=development nodemon app" to the scripts object in package.json. Using the dev module cross-env to automatically set the NODE_ENV environment variable on the machine the app will run on. Also, using nodemon for development.
```bash
    npm run start # production mode
    npm run dev # development mode (nodemon)
```

Created config directory, containing the config.env file (which will not be added to source control).

Using morgan for development only so the app logs more information about the requests the app serves and the time it needs to do so.

