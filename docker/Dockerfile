# 使用 Node 20-alpine 镜像作为基础镜像
FROM node:20-alpine

# 设置工作目录
WORKDIR /app

# 复制所有应用代码到容器中
COPY . .

# 暴露端口（假设应用监听3000端口）
EXPOSE 3000

# 启动应用（如果是 Node.js 应用，确保 worker.js 是入口文件）
CMD ["node", "worker.js"]
