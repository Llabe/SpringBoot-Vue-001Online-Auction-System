# 在线拍卖系统 / Online Auction System
---

![SpringBoot](https://img.shields.io/badge/SpringBoot-2.x-brightgreen)
![MyBatisPlus](https://img.shields.io/badge/MyBatisPlus-2.3-orange)
![Shiro](https://img.shields.io/badge/Shiro-1.3.2-blue)
![License](https://img.shields.io/badge/License-Apache2.0-orange)

---
# 项目简介  
基于SpringBoot + MyBatisPlus + Shiro的在线拍卖平台，包含商品管理、竞拍订单、历史记录和消息通知功能，支持前后端分离架构与鉴权控制。

# 特征介绍  
- ​**权限控制**：集成Shiro实现接口级权限验证，支持自定义鉴权注解（@IgnoreAuth）  
- ​**高效开发**：MyBatisPlus自动生成CRUD操作，XML映射文件与DAO层解耦  
- ​**文件管理**：独立FileController处理文件上传，集成百度AI工具类（BaiduUtil）  
- ​**模块化架构**：实体层细分VO/View/Model结构，支持多维度数据展示  
- ​**工具集成**：Hutool工具包处理通用逻辑，Fastjson实现高效JSON序列化  
---

# 代码结构 
```
src/
├── main/
│   ├── java/
│   │   ├── com/
│   │   │   ├── annotation/          # 权限注解
│   │   │   ├── config/              # 全局配置
│   │   │   │   ├── InterceptorConfig.java
│   │   │   │   ├── MybatisPlusConfig.java
│   │   │   ├── controller/          # 接口层
│   │   │   │   ├── FileController.java
│   │   │   │   ├── JingpaidingdanController.java
│   │   │   ├── dao/                 # 数据访问层
│   │   │   ├── entity/              # 数据模型
│   │   │   │   ├── model/           # 业务模型
│   │   │   │   ├── view/            # 视图模型
│   │   │   │   ├── vo/              # 值对象
│   │   │   ├── interceptor/         # 请求拦截器
│   │   │   ├── service/             # 服务层
│   │   │   │   ├── impl/            # 服务实现
│   │   │   ├── utils/               # 工具类
│   │   │   │   ├── BaiduUtil.java
│   │   │   │   ├── FileUtil.java
│   ├── resources/
│   │   ├── mapper/                  # MyBatis映射文件
│   │   ├── application.yml          # 主配置
│   │   ├── static/                  # 静态资源
│   │   │   ├── upload/              # 文件存储
```
---

# 使用说明
1. 数据库配置：修改application.yml中的MySQL连接信息
2. 启动项目：SpringbootSchemaApplication.java为主入口类
3. 访问地址：
   - 后台管理：http://localhost:8080/springbootp0eo6/admin/dist/index.html 
   - 前台系统：http://localhost:8080/springbootp0eo6/front/index.html
4. 管理员账号：abo/abo
5. 推荐运行环境：谷歌浏览器

# 技术文档
* 核心框架：[Spring Boot](https://spring.io/projects/spring-boot)
* 持久层框架：[MyBatisPlus](https://mp.baomidou.com)
* 权限认证：[Apache Shiro](https://shiro.apache.org)
* 工具套件：[Hutool](https://hutool.cn)
* 文件处理：[Baidu AI SDK](https://ai.baidu.com/sdk)
* JSON处理：[Fastjson](https://github.com/alibaba/fastjson)
* 验证框架：[JSR-303 Bean Validation](https://beanvalidation.org)
---

# 捐赠
> 博主将持续更新Java全栈开发项目，包含ssm，springboot，前后端分离系统等项目。
> 此外如果您够宽裕，请博主喝杯咖啡吧！捐赠将用于服务器维护与开源社区建设，感谢您的认可！
> 如需更多Java相关项目毕设3000+，sql文件可联系博主v:xq-lucky311
![输入图片说明](%E7%91%9E%E5%B9%B8%EF%BC%81%E7%91%9E%E5%B9%B8%EF%BC%81.png)
