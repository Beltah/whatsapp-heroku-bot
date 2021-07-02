# WhatsApp Heroku Bot

Uses [venom-bot](https://github.com/orkestral/venom)



## Deploying to heroku

1.  Fork this repo

2.  Clone it locally
```console
git clone https://github.com/YOUR_GITHUB_USER_NAME/whatsapp-heroku-bot
```

3.  Enter the folder
```console
cd whatsapp-heroku-bot
```

4.  If you haven't installed [Heroku](https://www.heroku.com/home) CLI yet, do it [here](https://devcenter.heroku.com/articles/heroku-cli).

5.  If you haven't logged in yet:
```console
heroku login
```

6.  Create a new Heroku app
```console
heroku create your-app-name
```

7.  Add [@heroku](https://github.com/heroku)'s `nodejs` buildpack. Docs [here](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-nodejs).
```console
heroku buildpacks:set heroku/nodejs
```

8.  Add [@jontewks](https://github.com/jontewks)'s `puppeteer` buildpack. Docs [here](https://elements.heroku.com/buildpacks/jontewks/puppeteer-heroku-buildpack).
```console
heroku buildpacks:add jontewks/puppeteer
```

9.  Add a remote to your repo.
```console
heroku git:remote -a your-app-name
```

10. Deploy your app to Heroku. This might take a while.
```console
git push heroku main
```

11. Do
```console
heroku logs
```
until you see the QR code. Scan it from `WhatsApp` in your phone.

12. It should be working!



## Running locally

1.  Fork this repo

2.  Clone it locally
```console
git clone https://github.com/YOUR_GITHUB_USER_NAME/whatsapp-heroku-bot
```

3.  Enter the folder
```console
cd whatsapp-heroku-bot
```

4.  Install npm dependencies
```console
npm install
```

5.  Run index.js
```
node index.js
```
or
```console
npm start
```

6. Wait until you see the QR code. Scan it from `WhatsApp` in your phone.

7. It should be working!


Venom bot documentation [here](https://orkestral.github.io/venom/index.html).