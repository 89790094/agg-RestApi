## Install && Config && Deploy
### Install
  Init:
  * mkdir/cd ProjectCatalog
  * npm init
  * npm i egg --save
  * npm i egg-bin --save--dev
  * npm run dev

  Add egg-bin:
  1. Edit Port -> package.json:  "scripts": {"dev": "egg-bin dev"}
	2. Open Brower -> http://localhost:7001
### Config
  1. package.json

    - Edit Port -> package.json:  "scripts": {"dev": "egg-bin dev --port PORT"}
    - 
  2. config/plugin.js
    - Install Plugin
      * cnpm i PlugName --save/auto update to package.json
    - Enable Plugin
      * Mongoose/mongodb
        > mysql: {enable: true,package: 'egg-mongoose'}
      * Mysql
        > mysql: {enable: true,package: 'egg-mysql'}
      * Validate
        > mysql: {enable: true,package: 'egg-validate'}
      * Sequelize/(mysql, mariadb, postgres, mssql)
        > sequelize:{enable: true,package: 'egg-sequelize'}
      * Schedule
        > schedule:{enable: true,package: 'egg-schedule'}
      * Jwt
        > jwt:{enable: true,package: 'egg-jwt'}
      * Redis
        > redis:{enable: true,package: 'egg-redis'}
  3. config/config.default.js
    - Add Jwt secret -> 'your key'
     
### Deploy

----
QQ:89790094
	

 
