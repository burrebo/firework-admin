# firework-admin

>An admin portal based on Spring MVC + Spring Security + MyBatis + Angularjs + Bootstrap + D3.js

- [Tutorial](https://fireworkstudio.github.io/firework-admin/en/)
- [中文介绍](https://github.com/fireworkstudio/firework-admin/tree/master/README-zh.md)

## Features:

* Manipulate multiple databases at backend.
* User-Role binding support.
* Each rest API with authentication check.
* Client-Side / Server-Side datatables pagination support.
* Easy to create Bar/Pie/Line charts.
* Multi maven profiles support.
* Junit support.
* Spring MVC + Spring Security + Mybatis + AngularJS stack.


## Install:
* Add following section in maven's settings.xml:

```xml
 <profiles>
    <profile>
        <id>myProfile</id>
        <repositories>
            <repository>
                <id>myRepository</id>
                <name>FireworkStudio</name>
                <url>http://fireworkstudio.cn:8081/nexus/content/repositories/thirdparty</url>
            </repository>
        </repositories>
    </profile>
  </profiles>

  <activeProfiles>
    <activeProfile>myProfile</activeProfile>
  </activeProfiles>
```
* Using `firework1.sql` and `firework2.sql` (in schema folder) to initialize two databases
* Database username/password could be changed in root `pom.xml`
* Run `mvn clean install -P develop`
* Deploy api.war `(/api)` and admin.war `(/admin)` in tomcat. (If you don't want `8080` port, you may modify `constant.js`)
* Access [http://localhost:8080/admin](http://localhost:8080/admin) via Chrome/Firefox, login name: `demo`, password: `demo`

### Build Environment (Recommend):
* Maven 3
* JDK 8

## Screenshots:
![image](http://7xknr8.com1.z0.glb.clouddn.com/asset/resource/20161007232234.jpg)

![image](http://7xknr8.com1.z0.glb.clouddn.com/asset/resource/20161014111628.jpg)

![image](http://7xknr8.com1.z0.glb.clouddn.com/asset/resource/20161016140309.jpg)

![image](http://7xknr8.com1.z0.glb.clouddn.com/asset/resource/20161016140326.jpg)

## License:

License under [Apache 2.0 license](http://opensource.org/licenses/Apache-2.0)

## References:

firework-admin benefits from these projects:

* [mybatis-cobarclient](https://github.com/aqqwiyth/mybatis-cobarclient)
* [angular-ui](https://github.com/angular-ui/bootstrap/)
* [angular-datatables](https://github.com/l-lin/angular-datatables)
* [angular-charts](https://github.com/chinmaymk/angular-charts)
* [angular-toolkits](https://github.com/shaunxu/angular-toolkits)
* [angular-busy](https://github.com/cgross/angular-busy)
* [angular-popups](https://github.com/aui/angular-popups)
* [angular-multi-select](https://github.com/alalonde/angular-multi-select)
* [angular-moment](https://github.com/urish/angular-moment)
* [angular-md5](https://github.com/gdi2290/angular-md5)