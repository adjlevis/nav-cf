# 使用 Node 20-alpine 镜像作为基础镜像
FROM node:20-alpine

# 设置工作目录
WORKDIR /app

# 复制 package.json 和 package-lock.json
COPY package.json package-lock.json ./

# 安装生产依赖
RUN npm install --production

# 复制应用代码
COPY . .

# 暴露端口（假设应用使用3000端口）
EXPOSE 3000  # 如果使用其他端口，修改这里

# 启动命令（确保 worker.js 是应用的入口文件）
CMD ["node", "worker.js"]
