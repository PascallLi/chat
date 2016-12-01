# chat

# 安装需求

apt-get install redis-server
pip3 install python-redis gunicorn

保持服务一直在后台运行
history|grep gunicorn
nohup gunicorn -b 0.0.0.0:8000 --worker-class=gevent -t 9999 redischat:app &
