# aixmi-archetypes
## 如何构建
`mvn clean install package`
## 如何发布
`mvn deploy -P release`
## 如何使用
替换`<>`的内容后使用命令:<br>
```shell script
mvn archetype:generate  -DgroupId=<font color="red"><your-group-id></font> -DartifactId=<your-artifact-id> -Dversion=<your-version> -Dpackage=<your-pacakge> -DarchetypeArtifactId=aixmi-mvc-archetype -DarchetypeGroupId=io.github.aixmi -DarchetypeVersion=1.0-SNAPSHOT
```

## archetypes
### aixmi-mvc-archetype
如:<br>
```shell script
mvn archetype:generate  -DgroupId=com.business -DartifactId=product-center -Dversion=1.0.0-SNAPSHOT -Dpackage=com.business.product -DarchetypeArtifactId=aixmi-mvc-archetype -DarchetypeGroupId=io.github.aixmi -DarchetypeVersion=1.0-SNAPSHOT
```
### aixmi-spring-boot-starter-archetype
```shell script
mvn archetype:generate  -DgroupId=io.github.aixmi -DartifactId=aixmi-spring-boot-starter-redis -Dversion=1.0.0-SNAPSHOT -Dpackage=io.github.aixmi.spring.boot.redis -DarchetypeArtifactId=aixmi-spring-boot-starter-archetype -DarchetypeGroupId=io.github.aixmi -DarchetypeVersion=1.0-SNAPSHOT
```

## FAQ
Q: 提示没有pom文件
A: 换一个终端
1. 分层
## reference
- [阿里巴巴COLA架构](https://github.com/alibaba/COLA)
- [阿里巴巴编码规约](https://github.com/alibaba/p3c)