赵忠赫
Go-后端开发工程师
求职 2004/11/26
zhaozhonghe@smail.sut.edu.cn 18545032297
https://blog.zhaozhonghe.me
教育经历
沈阳工业大学 电子与计算机工程 · 本科 · GPA 3.0 2023/9/9 - 2027/7/7
英语CET4

### 项目经历

银行项目管理 后端负责人 2024/6 - 2025/8
项目描述：基于 Go 语言构建的高性能银行核心系统，提供账户管理、交易转账等 API，系统采用容器化部
署，确保高可用和弹性伸缩。
技术栈：Go, Gin, PostgreSQL, Redis, Asynq, Docker, Kubernetes, GitHub Actions, JWT/PASETO
并发稳定性的验证： 利用 Go 语言的 Goroutine 机制 实现了高并发请求处理，并通过 PostgreSQL 事务锁
机制，在本机模拟高负载场景下进行了稳定性测试，验证了在高并发 I/O 场景下数据一致性和并发处理逻辑
的正确性。

性能基线测试与调优： 使用本地环境进行性能基线测试。通过对比发现，引入 Redis 缓存后，将核心 API
的平均响应延迟从 200ms 降低至 40ms，实现了 400% 的性能提升。

安全认证与权限控制：采用 PASETO/JWT 令牌实现无状态认证，并结合 Bcrypt 加密存储用户敏感信息。
DevOps 与自动化部署： 使用 Docker 对应用进行容器化，并通过 GitHub Actions 自动化构建、推送到
AWS ECR，实现了持续集成（CI）。高可用与弹性部署： 应用部署至 AWS EKS 集群，利用 Kubernetes
实现了服务的滚动更新和高可用。具备对 Deployment 和 Service 等核心资源的配置能力。

异步解耦与系统弹性：引入 Asynq 异步任务队列，极大地提升了核心交易 API 的响应速度和系统的容错
性。

工程质量与代码规范：利用 SQLC 实现 SQL 代码生成，保证了类型安全并减少了手动编写样板代码的错
误。通过 Gomock 完成核心业务逻辑的单元测试，覆盖率达 80%，确保代码质量。

### 专业技能

计算机基础: 熟悉计算机网络如 TCP 三次握手四次挥手、流量控制、超时重传、TLS 握手等；日常使用
Linux 系统 进行开发，了解 Linux 常用命令和基本操作系统知识；熟悉基本数据结构算法

编程语言： Golang,熟悉 goroutine，channel，select，context，GMP 模型 go 协程并发机制，熟悉 GC
算法；熟 悉 Go 语言中 map 等内置结构的实现

框架与中间件:： 熟悉 grpc框架基本使用；了解 Postgres 关系型数据库，了解数据库基本知识如 锁、索
引、事务、隔离机制等；了解 Redis 
