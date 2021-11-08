# 本地部署后端流程

---

1. [安装 Docker Compose](https://docs.docker.com/compose/install/)
2. 确保 .env 文件为如下内容
   ```.env
   DATABASE_URL="postgresql://postgres:admin@localhost:5432/maindbstaging"
   ```
3. 通过 docker-compose 安装 PostgreSQL 镜像到本地
   ```
   docker-compose up -d
   ```
4. 执行 npm install
   ```
   npm install
   ```
5. 执行数据库 migration
   ```
   prisma migrate dev
   ```
6. 启动后端服务器
   ```
   sh run.sh
   ```
7. 启动成功

   ```
   xtrmtek-backend % sh run.sh
   > xtrmtek-backend@1.0.0 dev
   > nodemon ./src/index.ts

   [nodemon] 2.0.14
   [nodemon] to restart at any time, enter `rs`
   [nodemon] watching path(s): *.*
   [nodemon] watching extensions: ts,json
   [nodemon] starting `ts-node ./src/index.ts`
   Example app listening at http://localhost:4000
   ```
