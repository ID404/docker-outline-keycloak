# docker-outline-keycloak
通过docker compose部署基本keycloak OIDC认证的outline服务

分二步部署
* 部署keycloak OIDC服务器
* 部署outline

# keycloak OIDC部署
1.进入keycloak文件夹，替换docker-compose.yaml文件中域名www.test.cn自己的域名

2.执行docker compose up -d 运行keycloak

3.登录http://www.test.cn:4430/ ,进入administratoration Console
[admin console](./images/admi-console.png)

添加client并记录OIDC client id 、OIDC client secret


# outline部署
4.进入outline文件夹，修改.env文件，替换www.test.cn域名为你自己的域名

5.修改.env文件中OIDC信息

6.docker compose up -d
