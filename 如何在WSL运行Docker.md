### 问题
直接在WSL中安装Docker是不行的，缺少docker demon进程。

### 实现步骤
##### 开启[Hyper-V](https://yeasy.gitbooks.io/docker_practice/install/windows.html)
##### 安装Docker Desktop
官网[docker](https://www.docker.com/)下载安装Docker Desktop
##### 设置守护服务
settings->General->Expose daemon on tcp://localhost:2375 without TSL
##### WSL中安装docker-ce
sudo apt install docker-ce
##### 设置环境变量
export DOCKER_HOST=tcp://127.0.0.1:2375
##### 测试
docker run hello-world

### 参考
[Docker — 从入门到实践](https://yeasy.gitbooks.io/docker_practice/)
[在Linux的Windows子系统上(WSL)使用Docker（Ubuntu）](https://www.cnblogs.com/xiaoliangge/p/9134585.html)
