# 使用 process manager（如 PM2）

`PM2` 是一个流行的 Node.js 进程管理器，专为 Node.js 应用服务，提供了监控、日志、自动重启等功能。

## 安装 PM2：

```Bash
npm install -g pm2
```

## 使用 PM2 ：

1. 启动你的 Node.js 应用：

```Bash
pm2 start server.js
```

2. 你可以通过以下命令查看正在运行的应用列表：

```Bash
pm2 list
```

3. 当你退出 SSH 连接时，PM2 会继续保持应用程序运行。

4. 重新连接后，你可以使用以下命令查看日志：

```Bash
pm2 logs
```

5. 你可以使用以下命令停止、重启或删除应用程序：

```Bash
pm2 stop <app_id|app_name> 
pm2 restart <app_id|app_name> 
pm2 delete <app_id|app_name>
```