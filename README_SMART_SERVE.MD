# 智柜通-SmartServe

## 目录结构

### 主要目录说明：

api/: 包含所有后端服务的代码，使用 Python 和 Flask 框架。负责处理业务逻辑、数据存储、模型调用等。
web/: 包含所有前端用户界面的代码，使用 TypeScript、React 和 Next.js 构建。负责用户交互和数据展示。
docker/: 包含用于构建和运行整个应用程序（包括前后端、数据库、中间件等）的 Docker 配置。
dev/: 包含开发者在本地开发和测试时使用的脚本和工具。
sdks/: 提供了不同语言的 SDK，方便开发者将 Dify 集成到自己的应用中。
images/: 存放项目文档或界面中使用的静态图片。
根目录文件: 包含项目的基础信息，如 README、许可证、贡献指南和构建脚本 (Makefile)。

### 目录结构说明：

```
.
├── api/             # 后端 API 代码 (Python/Flask)
│   ├── configs/       # 配置文件目录
│   ├── constants/     # 常量定义目录
│   ├── contexts/      # 上下文管理相关代码
│   ├── controllers/   # API 控制器 (路由处理)
│   ├── core/          # 核心业务逻辑
│   ├── docker/        # API 服务的 Docker 相关文件
│   ├── events/        # 事件处理相关代码
│   ├── extensions/    # Flask 扩展和自定义扩展
│   ├── factories/     # 工厂模式相关代码
│   ├── fields/        # API 请求/响应字段定义
│   ├── libs/          # 辅助库和工具函数
│   ├── migrations/    # 数据库迁移脚本 (Alembic)
│   ├── models/        # 数据库模型 (SQLAlchemy)
│   ├── schedule/      # 定时任务相关代码
│   ├── services/      # 业务服务层代码
│   ├── tasks/         # Celery 异步任务
│   ├── templates/     # 邮件模板等
│   └── tests/         # 后端测试代码
├── dev/             # 开发环境相关脚本和配置
│   └── pytest/        # Pytest 测试相关脚本
├── docker/          # Docker 部署相关配置
│   ├── certbot/       # Certbot (HTTPS 证书) 相关配置
│   ├── couchbase-server/ # Couchbase 服务配置
│   ├── elasticsearch/ # Elasticsearch 服务配置
│   ├── nginx/         # Nginx 反向代理配置
│   ├── pgvector/      # PgVector (PostgreSQL 向量扩展) 配置
│   ├── ssrf_proxy/    # SSRF 代理配置
│   ├── startupscripts/ # 启动脚本
│   ├── tidb/          # TiDB 相关配置
│   └── volumes/       # Docker 数据卷配置示例
├── images/          # 项目中使用的图片资源
├── sdks/            # 提供给开发者的软件开发工具包
│   ├── nodejs-client/ # Node.js SDK
│   ├── php-client/    # PHP SDK
│   └── python-client/ # Python SDK
├── web/             # 前端 Web 界面代码 (TypeScript/React/Next.js)
│   ├── __mocks__/     # Jest 测试 Mock 文件
│   ├── app/           # Next.js App Router 核心目录
│   ├── assets/        # 前端静态资源 (如图标)
│   ├── bin/           # 前端构建相关脚本
│   ├── config/        # 前端配置文件
│   ├── context/       # React Context API 相关代码
│   ├── docker/        # 前端服务的 Docker 相关文件
│   ├── hooks/         # React Hooks
│   ├── i18n/          # 国际化 (i18n) 语言文件
│   ├── models/        # 前端数据模型定义
│   ├── public/        # Next.js 公共静态资源
│   ├── service/       # 前端 API 服务请求封装
│   ├── styles/        # 全局样式文件
│   ├── themes/        # 主题样式 (亮色/暗色)
│   ├── types/         # TypeScript 类型定义
│   └── utils/         # 前端工具函数
├── AUTHORS          # 项目贡献者列表
├── CONTRIBUTING.md  # 贡献指南 (英文及多语言)
├── LICENSE          # 项目许可证 (Apache 2.0)
├── Makefile         # 项目构建和管理命令
└── README.md        # 项目介绍文档 (英文及多语言)

```