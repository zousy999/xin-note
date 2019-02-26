1. 配置管理角色  `conf/tomcat-users.xml`

```
<tomcat-users>

    <role rolename="manager-gui"/>
    <user username="admin" password="admin" roles="manager-gui"/>
</tomcat-users>
```



2.修改访问全选，如无新建 `conf/Catalina/localhost/manager.xml`

```
<Context privileged="true" antiResourceLocking="false"
         docBase="${catalina.home}/webapps/manager">
    <Valve className="org.apache.catalina.valves.RemoteAddrValve" allow="^.*$" />
</Context>
```



