# eCommerce - SoulWear

## Create tables from console:
```
// COMMANDS ON CONSOLE TO CREATE MODELS

sequelize model:generate --name User --attributes username:string,firstName:string,lastName:string,email:string,password:string,role:string,birthDate:date,gender:enum

sequelize model:generate --name Category --attributes name:string

sequelize model:generate --name Product --attributes name:string,price:float,description:string,CategoryId:int

sequelize model:generate --name Order --attributes date:date,status:enum,UserId:int

sequelize model:generate --name Detail --attributes OrderId:int,ProductId:int,quantity:int

sequelize model:generate --name Review UserID:int,ProductId:int
```