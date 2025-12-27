# 使用 Node 20-alpine 作为基础镜像
FROM node:20-alpine

# 设置工作目录
WORKDIR /app

# 复制依赖描述文件
COPY package.json package-lock.json ./

# 安装生产依赖
RUN npm install --production

# 复制应用源码
COPY . .

# 确保应用暴露正确的端口
EXPOSE 3000  # 如果应用使用其他端口，请修改这里

# 启动命令（确保 worker.js 是应用的正确入口文件）
CMD ["node", "worker.js"]
