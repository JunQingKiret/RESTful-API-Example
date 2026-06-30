# RESTful API 全流程交互演示

以 Todo 资源为例，展示 RESTful API 的端点定义、HTTP 请求/响应报文、资源状态机变迁。

## 使用方法

直接打开 `index.html` 即可运行，所有 API 逻辑均在浏览器端模拟，无需后端。

## 部署到 GitHub Pages

1. 将本项目推送到 GitHub 仓库的 `main` 分支
2. 进入仓库 Settings → Pages → Source 选择 **GitHub Actions**
3. 推送后 Actions 会自动构建并部署
4. 访问 `https://<username>.github.io/<repo-name>/`

## 功能

| 操作 | HTTP 方法 | 端点 | 说明 |
|------|-----------|------|------|
| 创建 | POST | /api/todos | 新建待办事项 |
| 查询全部 | GET | /api/todos | 返回所有资源 |
| 查询单个 | GET | /api/todos/:id | 返回指定资源 |
| 更新(全量) | PUT | /api/todos/:id | 重新激活资源 |
| 更新(部分) | PATCH | /api/todos/:id | 标记完成 |
| 删除 | DELETE | /api/todos/:id | 删除资源 |

## 状态机
