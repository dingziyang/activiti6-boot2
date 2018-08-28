# activiti6-boot2
修改activiti-tag6.0的官方源码，以兼容springboot2，故定义为boot2版本

## 环境
- spring-boot2.0.2 ，如需改为其它2.x版本，请注意更改pom中对应的spring其它组件的版本

#### 在modules\activiti-ui和modules\activiti-spring-boot下，分别运行以下命令（按顺序）(本项目源码是已经运行好了的)
 - mvn versions:set -DnewVersion=6.0.0-boot2
 - mvn clean install source:jar -Dmaven.test.skip=true

 
#### 本地安装和上传私服
1. 在modules\activiti-ui和modules\activiti-spring-boot下，先后分别```mvn clean install -Dmaven.test.skip=true```
2. 在modules\activiti-ui和modules\activiti-spring-boot下，先后分别```mvn deploy -Dmaven.test.skip=true```