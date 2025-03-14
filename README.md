整个项目名称为：springboot001基于SpringBoot的在线拍卖系统，接下来我会给你一个完整的项目目录结构和 pom.xml 文件，希望你能帮我完成以下任务：

1.生成项目介绍与特征
需求说明：
	以项目名称为主，结合pom.xml 中的依赖和目录结构，提炼技术栈和功能特性。
​输出内容：
	· 项目标题：项目名称中文 / 项目名称英文(项目名称去除技术栈信息保留核心主题)。
	· 项目相关技术：根据pom自行提取前后端核心技术与版本。
	​· 项目简介：概括项目类型、技术组成和核心功能。
	​· 特征介绍：用分点列表描述技术亮点和设计优势。
示例输出：
# 智慧物流管理系统 / Intelligent logistics management
---

![SpringBoot](https://img.shields.io/badge/SpringBoot-2.7%2B-brightgreen)
![Vue](https://img.shields.io/badge/Vue-2.x-4fc08d)
![License](https://img.shields.io/badge/License-Apache2.0-orange)

---
# 项目简介  
基于 SpringBoot + Mybatis Plus + SaToken 的后台管理系统，支持 RBAC 权限控制、代码生成器和多数据源切换，适用于快速开发企业级应用。


# 特征介绍  
- ​**权限控制**：集成 Sa-Token 实现角色/菜单动态权限，支持前后端分离鉴权。  
- ​**高效开发**：MyBatis-Plus 零 SQL 实现单表操作，提供 MySQL/Oracle 代码生成器。  
- ​**多数据源**：通过 `@DS` 注解自由切换数据库，支持 Druid 连接池监控。  
- ​**接口文档**：集成 Knife4j 自动生成 API 文档，符合 RESTful 规范。  
- ​**精简架构**：SpringBoot 脚手架结构，模块化设计便于二次开发。  
---

2.代码结构
核心功能目录保留：
​	1.后端核心结构：
		· 保留与业务逻辑、数据持久化、接口处理相关的目录：
		· controller（接口处理层，示例文件：UserController.java）
		· service（业务逻辑层，示例文件：UserService.java + UserServiceImpl.java）
		· entity（数据模型层，示例文件：User.java）
		· mapper 或 dao（数据持久化层，示例文件：UserMapper.xml）
		· config（全局配置类，示例文件：SecurityConfig.java）
		· utils（公共工具类，示例文件：CommonUtil.java）
		· 保留项目启动类（如 Application.java）和核心配置文件（如 application.yml）。
​	2.前端核心结构：
		· 保留与页面渲染、路由、状态管理相关的目录：
		· views/pages（页面目录，示例文件：UserList.vue）
		· components（组件目录，示例文件：UserCard.vue）
		· router（路由配置，示例文件：index.js）
		· store（状态管理，示例文件：store.js）
		· assets（静态资源目录，保留 css、js、images 子目录）。
​	3.非核心目录移除：
		· 移除临时文件（.bak）、第三方库（bootstrap/jquery）、开发工具文件（.bat/package.json）等。
演示实例：
# 代码结构 
	src/
	├── main/
	│   ├── java/
	│   │   ├── com/
	│   │   │   ├── annotation/          # 鉴权注解
	│   │   │   ├── config/              # 全局配置
	│   │   │   ├── controller/          # 接口层
	│   │   │   │   ├── CangkuController.java
	│   │   │   │   ├── FileController.java
	│   │   │   ├── dao/                 # 数据访问层
	│   │   │   ├── entity/              # 数据模型
	│   │   │   │   ├── model/           # 业务模型
	│   │   │   ├── interceptor/         # 请求拦截器
	│   │   │   ├── service/             # 服务层
	│   │   │   │   ├── impl/            # 服务实现
	│   │   │   ├── utils/               # 工具类
	│   ├── resources/
	│   │   ├── mapper/                  # MyBatis映射文件
	│   │   ├── application.yml          # 主配置
	│   │   ├── log4j.properties         # 日志配置
	│
	├── webapp/
	│   ├── src/
	│   │   ├── assets/                  # 静态资源
	│   │   │   ├── css/
	│   │   │   ├── img/  
	│   │   ├── components/              # 公共组件
	│   │   │   ├── common/              # 通用组件
	│   │   ├── router/                  # 路由配置
	│   │   ├── store/                   # 状态管理
	│   │   ├── views/                   # 业务页面
	│   │   │   ├── modules/             # 功能模块
	│   │   │   │   ├── cangku/          # 仓库管理
	│   │   │   │   ├── jiesuan/         # 结算管理

---

# 使用说明
需求说明：
	把需处理内容的说明文档信息结合上诉信息完善进行输出即可
---	

# 技术文档
需求说明：
	结合上诉信息，对核心技术栈信息汇总
实例输出：
* 核心框架：[Spring Boot](https://spring.io/projects/spring-boot)
* 持久层框架：[MyBatis-Plus](https://mybatis.plus)
* 权限认证：[Sa-Token](https://sa-token.cc/doc.html#/)
* 前端框架: [Layui](https://layui.dev/docs/2/)
* 数据库连接池：[Alibaba Druid](https://github.com/alibaba/druid/)
* 模板引擎：[Thymeleaf](https://www.thymeleaf.org/)
---

捐赠(注：这模块内容不变)
# 捐赠
    > 博主将持续更新Java全栈开发项目，包含ssm，springboot，前后端分离系统等项目。
    > 此外如果您够宽裕，请博主喝杯咖啡吧！捐赠将用于服务器维护与开源社区建设，感谢您的认可！
    > 如需更多Java相关项目毕设3000+，sql文件可联系博主v:xq-lucky311
![输入图片说明](%E7%91%9E%E5%B9%B8%EF%BC%81%E7%91%9E%E5%B9%B8%EF%BC%81.png)
---

总体要求：	
	1.不要生成带解释说明信息，如："第一步", "简化", "移除内容"等字样；
	2.输出结果：只有开头和结尾用```符号，中间不要出现；
		尤其是在"代码结构","yaml","技术文档"模块附近不要出现`符号；
​请处理以下内容：
目录结构:
├── mvnw
├── mvnw.cmd
├── pom-war.xml
├── pom.xml
├── src
    ├── main
        ├── java
            ├── com
                ├── SpringbootSchemaApplication.java
                ├── annotation
                    ├── APPLoginUser.java
                    ├── IgnoreAuth.java
                    ├── LoginUser.java
                ├── config
                    ├── InterceptorConfig.java
                    ├── MybatisPlusConfig.java
                ├── controller
                    ├── CommonController.java
                    ├── ConfigController.java
                    ├── FileController.java
                    ├── JingpaidingdanController.java
                    ├── LishijingpaiController.java
                ├── dao
                    ├── CommonDao.java
                    ├── ConfigDao.java
                    ├── JingpaidingdanDao.java
                    ├── LishijingpaiDao.java
                    ├── MessagesDao.java
                ├── entity
                    ├── ConfigEntity.java
                    ├── EIException.java
                    ├── JingpaidingdanEntity.java
                    ├── LishijingpaiEntity.java
                    ├── MessagesEntity.java
                    ├── model
                        ├── JingpaidingdanModel.java
                        ├── LishijingpaiModel.java
                        ├── MessagesModel.java
                        ├── NewsModel.java
                        ├── PaimaishangpinModel.java
                    ├── view
                        ├── JingpaidingdanView.java
                        ├── LishijingpaiView.java
                        ├── MessagesView.java
                        ├── NewsView.java
                        ├── PaimaishangpinView.java
                    ├── vo
                        ├── JingpaidingdanVO.java
                        ├── LishijingpaiVO.java
                        ├── MessagesVO.java
                        ├── NewsVO.java
                        ├── PaimaishangpinVO.java
                ├── interceptor
                    ├── AuthorizationInterceptor.java
                ├── service
                    ├── CommonService.java
                    ├── ConfigService.java
                    ├── JingpaidingdanService.java
                    ├── LishijingpaiService.java
                    ├── MessagesService.java
                    ├── impl
                        ├── CommonServiceImpl.java
                        ├── ConfigServiceImpl.java
                        ├── JingpaidingdanServiceImpl.java
                        ├── LishijingpaiServiceImpl.java
                        ├── MessagesServiceImpl.java
                ├── utils
                    ├── BaiduUtil.java
                    ├── CommonUtil.java
                    ├── FileUtil.java
                    ├── HttpClientUtils.java
                    ├── JQPageInfo.java
        ├── resources
            ├── admin
                ├── admin
                    ├── 1-install.bat
                    ├── 2-run.bat
                    ├── 3-build.bat
                    ├── package-lock.json
                    ├── package.json
                    ├── public
                        ├── favicon.ico
                    ├── src
                        ├── App.vue
                        ├── assets
                            ├── css
                                ├── css
                            ├── img
                                ├── img
                        ├── components
                            ├── SvgIcon
                                ├── index.vue
                            ├── common
                                ├── BreadCrumbs.vue
                                ├── Editor.vue
                                ├── FileUpload.vue
                            ├── home
                                ├── HomeCard.vue
                                ├── HomeChart.vue
                                ├── HomeComment.vue
                                ├── HomeProgress.vue
                            ├── index
                                ├── index
                        ├── icons
                            ├── icons
                        ├── router
                        ├── store
                        ├── utils
                        ├── views
                            ├── views
                        ├── vm
                            ├── add-or-update.vue.vm
                            ├── base.js.vm
                            ├── http.js.vm
                            ├── list.vue.vm
                            ├── login.vue.vm
            ├── application.yml
            ├── front
                ├── front
                    ├── css
                        ├── css
                    ├── elementui
                        ├── elementui
                    ├── img
                        ├── img
                    ├── layui
                        ├── css
                            ├── css
                        ├── font
                            ├── font
                        ├── images
                            ├── images
                        ├── lay
                            ├── modules
                                ├── modules
                    ├── modules
                        ├── modules
                    ├── pages
                        ├── pages
                    ├── xznstatic
                        ├── css
                            ├── css
                        ├── img
                            ├── img
            ├── mapper
                ├── CommonDao.xml
                ├── ConfigDao.xml
                ├── JingpaidingdanDao.xml
                ├── LishijingpaiDao.xml
                ├── MessagesDao.xml
            ├── static
                ├── upload
                    ├── upload
    ├── test
        ├── test

POM 依赖项:
org.springframework.boot:spring-boot-starter-web:UNKNOWN
org.mybatis.spring.boot:mybatis-spring-boot-starter:2.1.1
org.springframework.boot:spring-boot-starter-jdbc:UNKNOWN
mysql:mysql-connector-java:UNKNOWN
org.apache.shiro:shiro-spring:1.3.2
com.baomidou:mybatis-plus:2.3
com.baomidou:mybatisplus-spring-boot-starter:1.0.5
com.google.protobuf:protobuf-java:3.10.0
org.apache.commons:commons-lang3:3.0
javax.validation:validation-api:2.0.1.Final
commons-io:commons-io:2.5
cn.hutool:hutool-all:4.0.12
com.alibaba:fastjson:1.2.8
com.baidu.aip:java-sdk:4.4.1
org.springframework.boot:spring-boot-starter-test:UNKNOWN

说明文档:
推荐使用：谷歌浏览器


后台地址
http://localhost:8080/springbootp0eo6/admin/dist/index.html

管理员  abo 密码 abo


前台地址：http://localhost:8080/springbootp0eo6/front/index.html


 
在src\main\resources\application.yml中编辑
											
	 url: jdbc:mysql://127.0.0.1:3306/springbootp0eo6?useUnicode=true&characterEncoding=utf-8&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone=UTC
        username: root
        password: 123456 （数据库密码）