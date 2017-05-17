## Welcome to Foxtrapp

Thank you for being a part of our professional team. This manifest describes our enterprise standards.
We are ready to consider your proposal upon reviewing and discussion of pull request.

## Web

Continuous integration and delivery according to [12 app factor](https://12factor.net).

1. Primary platform as a service [Heroku](https://heroku.com).
2. Primary continuous integration and delivery service [Codeship](https://codeship.com).
3. GitHub, Beanstalk
4. Node.js 6.5.0 and NPM 3.10.3

### Frontend

1. Primary framework [React.js](https://facebook.github.io/react/)
2. Angular 2
3. Backbone.js together with Marionnete.js
4. Bootstrap

### Backend

1. Primary framework [KOA](https://github.com/koajs/koa)
2. Primary database [Mongodb 3.4](https://www.mongodb.com/cloud/atlas)
3. Express

#### Internal event format

Primary format event approved according to *Schema Draft v4*

```
    {
        "title": "Event",
        "type": "object",
        "properties": {
            "headers": {
                "type": "object",
                "properties": {
                    "contentType": {
                        "type": "string"
                    },
                    "actionType": {
                        "type": "string"
                    },
                    "user": {
                        "type": "string"
                    }
                },
                "required": ["contentType", "actionType"]
            },
            "payload": {
                "type": "object",
                "properties": {}
            }
        },
        "required": ["headers", "payload"]
    }
```

### Services in cloud

 - MongoDB Atlas
 - RethinkDB Compose.io
 - Heroku Add-ons (Redis, RabbitMQ)
 - PubNub
 - AWS S3
 - SendGrid
 - Twilio
 - Firebase Cloud Messaging

### Enterprise solutions

 1. [ESLint config](https://github.com/oleksijfomin/eslint-config-udosoft)
 2. [Abstract scheduler](https://github.com/rhinobuccaneers/abstract-scheduler)
 3. [Heroku Buildpack Multi](https://github.com/rhinobuccaneers/heroku-buildpack-multi)
 4. [Heroku Buildpack FFMPEG](https://github.com/rhinobuccaneers/heroku-buildpack-ffmpeg)
 5. [Heroku Buildpack GraphicsMagic](https://github.com/foxtrapplimited/heroku-buildpack-graphicsmagick)

### Allowed node modules
```
async,aws-sdk,bluebird,body-parser,bower,bson-objectid,co,co-express,compression,connect-mongo,connect-multiparty,connect-redis,consolidate,cookie-parser,csurf,csvtojson,dotenv,express,express-request-id,express-session,fluent-ffmpeg,generate-password,handlebars,i18n,imagemagick,joi,joi-objectid,levee,lodash,moment,mongodb,mongodb-migrate,mongoose,morgan,multiparty,nconf,newrelic,node-gcm,node-mailer,node-schedule,nodemailer,nodemailer-sendgrid-transport,pubnub,redis,request,s3policy,shortid,socket.io,socket.io-redis,supertest-as-promised,swig,throng,twilio,underscore,validator,winston,xlsx,xss-filters,aglio,chai,chai-datetime,co-mocha,commitizen,cross-env,cz-conventional-changelog,eslint,eslint-config-udosoft,faker,grunt,grunt-jsdoc,istanbul,jsdoc,json-server,mocha,mocha-junit-reporter,mongo-xlsx,nyc,open,pre-push,shelljs,sinon,sinon-chai,supertest,supertest-session,axios,babel-polyfill,compact-object,cors,deep-copy,deep-equal,email-validator,express-winston,http-proxy-middleware,ip,json-loader,number-to-words,react,react-dom,react-redux,react-restricted-input,react-router,react-router-redux,react-slick,react-textarea-autosize,redux,redux-actions,redux-form,redux-localstorage,redux-logger,redux-saga,redux-thunk,slick-carousel,uuid,valid-url,validate.js,year-range-regex,axios-mock-adapter,babel-core,babel-eslint,babel-loader,babel-plugin-react-html-attrs,babel-plugin-transform-class-properties,babel-plugin-transform-decorators-legacy,babel-plugin-transform-react-jsx,babel-plugin-transform-runtime,babel-preset-es2015,babel-preset-react,babel-preset-react-hmre,babel-preset-stage-0,babel-runtime,chai-as-promised,css-loader,es6-promise,es6-shim,eslint-config-airbnb,eslint-plugin-import,eslint-plugin-jsx-a11y,eslint-plugin-react,extract-text-webpack-plugin,file-loader,html-webpack-plugin,istanbul-instrumenter-loader,jasmine-co,jasmine-core,karma,karma-chai,karma-coverage,karma-es6-shim,karma-jasmine,karma-jasmine-html-reporter,karma-phantomjs-launcher,karma-sinon,karma-spec-reporter,karma-webpack,less,less-loader,matchdep,nock,node-mock-server,node-sass,phantomjs-polyfill,phantomjs-prebuilt,react-addons-test-utils,react-hot-loader,react-styleguidist,redux-mock-store,style-loader,stylus,stylus-loader,svg-to-jsx,tap-spec,tape,url-loader,webpack,webpack-dev-middleware,webpack-dev-server,webpack-hot-middleware,@risingstack/trace,apidoc,http-status,is-progressive,koa,koa-66,koa-body,koa-convert,koa-helmet,koa-static,mime-kind,winston-mongodb,js-image-generator,nodemon,slack-shippable
```
