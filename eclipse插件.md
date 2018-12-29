安装
设置本地仓库
本地仓库 
文件在安装文件的/conf/settings.xml 
内容：通过配置 
否则默认本地仓库：${user.home}/.m2/repository

使用外部maven
选取

这里写图片描述

这里写图片描述

这里写图片描述

操作
updateProject
拉取 
编写完pom.xml以后, 
右键项目–>maven–>updateProject 
自动拉取jar包

mvn clean 清空生成的文件 
mvn compile 编译 
mvn clean compile 删除再编译

mvn test 编译并测试

mvn install 发布jar到本地仓库 
mvn install -DskipTests

eclipse运行组合命令 
选择项目—run as —maven build.. – 在goal中输入组合命令,不需要mvn

依赖
超级POM 和 自定义POM 
有效POM：管理项目时，最终使用的POM 
包括：超级POM 和 自定义POM 
超级POM：maven 提供的pom.xml (特定的内容) 
自定义POM：maven项目自己编写的pom.xml

dependency hierarchy 
依赖分层管理 
能够看到依赖的完整




Maven Helper
一键查看maven依赖，查看冲突的依赖，一键进行exclude依赖