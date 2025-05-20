# 全栈应用项目

这是一个使用FastAPI和Vite构建的前后端分离项目框架。

## 项目结构

```
.
├── backend/                # 后端项目目录
│   ├── app/               # 应用主目录
│   │   ├── api/          # API路由
│   │   ├── models/       # 数据模型
│   │   └── services/     # 业务逻辑
│   ├── requirements.txt   # Python依赖
│   └── main.py           # 应用入口
│
├── frontend/              # 前端项目目录
│   ├── src/              # 源代码
│   │   ├── components/   # Vue组件
│   │   ├── views/        # 页面视图
│   │   ├── router/       # 路由配置
│   │   ├── assets/       # 静态资源
│   │   ├── App.vue       # 根组件
│   │   └── main.js       # 入口文件
│   ├── public/           # 公共资源
│   ├── package.json      # 项目配置
│   └── vite.config.js    # Vite配置
│
└── README.md             # 项目说明
```

## 技术栈

### 后端
- Python 3.8+
- FastAPI
- MySQL
- Uvicorn

### 前端
- Node.js
- Vite
- Vue 3
- Vue Router

## 开发环境设置

### 环境要求
1. Node.js和npm
   - 检查是否已安装：
     ```bash
     node --version
     npm --version
     ```
   - 如果未安装：
     - Windows: 从[Node.js官网](https://nodejs.org/)下载安装
     - Mac: 使用Homebrew安装：`brew install node`
   - 安装完成后再次验证：
     ```bash
     node --version
     npm --version
     ```

### 后端设置
1. 进入backend目录:`cd backend`
2. 安装依赖：`pip install -r requirements.txt`
3. 运行服务：`uvicorn main:app --reload`

### 前端设置
1. 进入frontend目录：`cd frontend`
2. 安装依赖：`npm install`
3. 运行开发服务器：`npm run dev`

## API文档
启动后端服务后，访问以下地址查看API文档：
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## 开发指南

### 后端开发
1. 所有API路由定义在 `backend/app/api/` 目录下
2. 数据模型定义在 `backend/app/models/` 目录下
3. 业务逻辑实现在 `backend/app/services/` 目录下

### 前端开发
1. 组件开发在 `frontend/src/components/` 目录下
2. 页面视图在 `frontend/src/views/` 目录下
3. 路由配置在 `frontend/src/router/` 目录下

