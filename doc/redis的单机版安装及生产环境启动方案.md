### 1.单机版安装  
#### 1.1 下载  
wget http://download.redis.io/releases/redis-stable.tar.gz  
#### 1.2 解压  
tar zvxf redis-stable.tar.gz  
#### 1.3 安装  
make && make test  
make install PREFIX=/usr/local/redis  
#### 1.4 启动  
将redis.conf拷贝到redis的安装目录下:  
cp redis.conf /usr/local/redis/bin  
修改redis.conf,将daemonize no修改为daemonize yes,使用守护进程,即后台运行  
启动:  
./redis-server redis.conf  
#### 1.5 关闭  
./redis-cli shutdown
