# 使用 Node 20-alpine 作为基础镜像
FROM node:20-alpine

# 设置工作目录
WORKDIR /app

# 复制所有文件到容器中的工作目录
COPY . .

# 安装生产依赖
RUN npm install --production

# 暴露端口
EXPOSE 3000

# 启动命令，确保 node 和 worker.js 路径正确
CMD ["node", "worker.js"]
