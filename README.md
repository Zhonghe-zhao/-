# 我的简历

> 我的简历，求职使用，记录自己的一点点成长

###  赵忠赫

[3041322213@qq.com](mailto:3041322213@qq.com) | 📱 18545032297 | [blog](https://blog.zhaozhonghe.me)
 求职意向：Go 后端开发实习

------

### 教育背景

  **沈阳工业大学** - 电子与计算机工程 （2023.09 - 2027.06）

------

### 技术栈

  - **Golang**：熟练掌握 goroutines、channel、Worker Pool，理解GMP，垃圾回收机制，掌握单元测试。
  - **Web 框架**：熟悉使用 Gin、gorm理解中间件机制、参数绑定，。
  - **数据库**：熟练 PostgreSQL、Redis，掌握 SQL 、事务隔离、索引，熟悉 ACID。
  - **微服务通信**：熟悉 gRPC 与 Protocol Buffers，了解服务注册与高效通信。
  - **DevOps**：熟悉 Docker、docker-compose，能独立容器化部署服务；会使用 GitHub Actions 实现自动构建与部署。
  - **基础知识**：掌握操作系统线程模型、计算机网络 TCP/IP、HTTP协议。

------

### 项目经验

#### 银行系统（Simple Bank）

  **技术栈**：Go, Gin, PostgreSQL, Redis, Docker, sqlc, gRPC, Passeto
   **项目地址**：https://github.com/Zhonghe-zhao/Simple_bank
   **项目描述**：
   独立实现一个支持并发转账、账户管理、身份认证的简化银行系统。

  **关键成果**：

1. **实现账户、转账、查询等 RESTful API**，每日模拟请求量 > 2w，接口平均响应时间 < 30ms。

2. **自定义事务处理逻辑**，解决并发转账数据不一致和死锁的避免，**通过事务隔离级别+锁控制+事务执行顺序控制**。

3. **基于 sqlc 生成类型安全查询代码**，替代 ORM，查询效率提升约 25%。

4. **使用 Passeto 代替 JWT 实现身份认证**，减少 token 漏洞风险，支持 token 刷新与注销。

5. 使用 **gRPC + Protobuf** 封装内部 RPC 服务，支持模块解耦与服务扩展。

6. 项目使用 **Docker 一键部署**，并使用 GitHub Actions 实现自动构建镜像。

7. **使用 gRPC 重构用户相关接口**，替代传统 RESTful 实现，通过 `.proto` 文件统一定义接口与数据结构，实现接口代码自动生成与强类型校验。

​       当前项目未涉及服务间通信，但该设计为后续拆分微服务架构打下基础，**提升接口性能、可维护性与扩展性**。

