# mongo-cp
Mongo dashboard

Name                              | Default         | Description
----------------------------------|-----------------|------------
`ME_CONFIG_MONGODB_SERVER`        |`mongo` or `localhost`| MongoDB host name or IP address. The default is `localhost` in the config file and `mongo` in the docker image. If it is a replica set, use a comma delimited list of the host names.
`ME_CONFIG_MONGODB_PORT`          | `27017`         | MongoDB port.
`ME_CONFIG_MONGODB_URL`           | `mongodb://admin:pass@localhost:27017/db?ssl=false`
`ME_CONFIG_MONGODB_ENABLE_ADMIN`  | `false`         | Enable administrator access. Send strings: `"true"` or `"false"`.
`ME_CONFIG_MONGODB_ADMINUSERNAME` | ` `             | Administrator username.
`ME_CONFIG_MONGODB_ADMINPASSWORD` | ` `             | Administrator password.
`ME_CONFIG_MONGODB_AUTH_DATABASE` | `db`            | Database name (only needed if `ENABLE_ADMIN` is `"false"`).
`ME_CONFIG_MONGODB_AUTH_USERNAME` | `admin`         | Database username (only needed if `ENABLE_ADMIN` is `"false"`).
`ME_CONFIG_MONGODB_AUTH_PASSWORD` | `pass`          | Database password (only needed if `ENABLE_ADMIN` is `"false"`).
`ME_CONFIG_SITE_BASEURL`          | `/`             | Set the express baseUrl to ease mounting at a subdirectory. Remember to include a leading and trailing slash.
`ME_CONFIG_SITE_COOKIESECRET`     | `cookiesecret`  | String used by [cookie-parser middleware](https://www.npmjs.com/package/cookie-parser) to sign cookies.
`ME_CONFIG_SITE_SESSIONSECRET`    | `sessionsecret` | String used to sign the session ID cookie by [express-session middleware](https://www.npmjs.com/package/express-session).
`ME_CONFIG_BASICAUTH_USERNAME`    | `admin`         | mongo-express web login name. Sending an empty string will disable basic authentication.
`ME_CONFIG_BASICAUTH_PASSWORD`    | `pass`          | mongo-express web login password.
`ME_CONFIG_REQUEST_SIZE`          | `100kb`         | Used to configure maximum mongo update payload size. CRUD operations above this size will fail due to restrictions in [body-parser](https://www.npmjs.com/package/body-parser).
`ME_CONFIG_OPTIONS_EDITORTHEME`   | `rubyblue`      | Web editor color theme, [more here](http://codemirror.net/demo/theme.html).
`ME_CONFIG_SITE_SSL_ENABLED`      | `false`         | Enable SSL.
`ME_CONFIG_MONGODB_SSLVALIDATE`   | `true`          | Validate mongod server certificate against CA
`ME_CONFIG_SITE_SSL_CRT_PATH`     | ` `             | SSL certificate file.
`ME_CONFIG_SITE_SSL_KEY_PATH`     | ` `             | SSL key file.
`ME_CONFIG_SITE_GRIDFS_ENABLED`   | `false`         | Enable gridFS to manage uploaded files.
`VCAP_APP_PORT`                   | `8081`          | port that mongo-express will run on. 
