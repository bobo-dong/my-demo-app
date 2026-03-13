# My Demo App

演示 Kubernetes CI/CD 工作流的示例应用。

## 本地运行

```bash
npm install
npm start
```

访问 http://localhost:3000

## 工作流

1. 推送代码到 GitHub
2. Drone CI 自动构建 Docker 镜像
3. 镜像推送到 Docker Hub
4. 更新 K8s 配置仓库的镜像版本
5. Argo CD 自动部署到 K8s 集群
