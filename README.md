# FlyGo_Maven_Nexus
文档地址：https://www.flygo520.com/docs/maven/maven-1amv2ceq32pa9


工程里面的 `pom.xml` 配置文件，修改成你的私服地址

```bash
<distributionManagement>
		<repository>
			<!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
			<id>nexus-releases</id>
			<name>Nexus Release Repository</name>
			<url>http://${你的私服地址}/nexus/content/repositories/releases/</url>
		</repository>
		<snapshotRepository>
			<!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
			<id>nexus-snapshots</id>
			<name>Nexus snapshot Repository</name>
			<url>http://${你的私服地址}/nexus/content/repositories/snapshots/</url>
		</snapshotRepository>
	</distributionManagement>
```
  
  
 
