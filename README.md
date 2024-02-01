# docker-outline-keycloak
1.进入keycloak文件夹，替换docker-compose.yaml文件中域名www.test.cn自己的域名，保存

2.执行docker compose up -d

3.登录http://www.test.cn:4430/ ,添加client并记录OIDC client id 、OIDC client secret

4.进入outline文件夹，修改.env文件，替换www.test.cn域名为你自己的域名

5.修改.env文件中OIDC信息

6.docker compose up -d
