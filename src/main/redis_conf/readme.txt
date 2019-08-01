redis.conf为主库配置文件 port 6000
redis2.conf port 6002、redis3.conf port 6003为从库配置文件
主从库密码需一致 本文均为123456
sentinel.conf port 26479 为哨兵配置文件

分别启动主库、从库、哨兵
    redis-server redis.conf
    redis-server redis2.conf
    redis-server redis3.conf
    redis-server sentinel.conf --sentinel