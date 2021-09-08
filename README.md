# 本地部署后端流程

---

1. [下载并安装本地 PostgreSQL 数据库](https://www.prisma.io/dataguide/postgresql/setting-up-a-local-postgresql-database#overview)
   创建一个新的数据库， 名称为 `maindbstaging`， 用户名为 `postgres`， 密码为 `admin`
2. 确保 .env 文件为如下内容
   ```.env
   DATABASE_URL="postgresql://postgres:admin@localhost:5432/maindbstaging"
   ```
3. 执行数据库 migration
   ```
   prisma migrate dev
   ```
4. 启动后端服务器
   ```
   npm start
   ```
