# 使用Docker快速搭建基础环境

## 1.Nacos-docker

https://nacos.io/zh-cn/docs/quick-start-docker.html

- Clone 项目

  ```powershell
  git clone https://github.com/nacos-group/nacos-docker.git
  cd nacos-docker
  ```

- 单机模式 Derby

  ```powershell
  docker-compose -f example/standalone-derby.yaml up -d
  ```

- 单机模式 MySQL

​	如果希望使用MySQL5.7

```powershell
docker-compose -f example/standalone-mysql-5.7.yaml up -d
```

如果希望使用MySQL8

```powershell
docker-compose -f example/standalone-mysql-8.yaml up
```

- 集群模式

  ```powershell
  docker-compose -f example/cluster-hostname.yaml up 
  ```

## 2.Seata-docker

- 使用docker-compose启动

  ```powershell
  docker-compose -f docker-compose.yaml up -d
  ```

