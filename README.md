# Blinkin api strapi
Some of the blinkin api in strapi
1) Issue api

# Required env variable
1) For postgres

```js
 settings: {
        client: "postgres",
        host: "${process.env.DATABASE_HOST || '127.0.0.1'}",
        port: "${process.env.DATABASE_PORT || 27017}",
        database: "${process.env.DATABASE_NAME || 'strapi'}",
        username: "${process.env.DATABASE_USERNAME || ''}",
        password: "${process.env.DATABASE_PASSWORD || ''}"
      },
```
2) for jwt verify
```js
process.env.JWT_SECRET
```

# Steps
```js
git clone -b issue-api https://github.com/ranjith29v/strapi-blinkin-api.git  
cd strapi-blinkin-api  
npm install  
NODE_ENV=production npm run build  
npm start  
```
for detail deployment option https://strapi.io/documentation/3.0.0-beta.x/deployment/amazon-aws.html
