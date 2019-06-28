# tiger
hello world
ceph-deploy new node1 node2 node3定义监视器及主机
ceph-deploy mon create-initial 开启服务
ceph-deploy disk zap node1:vdc node1:vdd 格式化某盘
ceph-deploy disk zap node2:vdc node1:vdd 格式化某盘
ceph-deploy dis zap 主机名：硬盘
ceph-deploy osd create 主机名：硬盘：缓存盘
ceph-deploy mds create node4 给node4拷贝配置文件，启动mds服务
ceph -s 查看状态
ceph osd lspools 查看地址池
rbd create 镜像名 --image-feature layering --szie 10G 创建镜像
rbd list列出镜像
rbd info 镜像名查看镜像信息
rbd resize --size 7G 镜像名 --allow-shrink 容量调整
rbd resize --size 50G 镜像名 
rbd map 镜像名 使用镜像
rbd showapped 查看镜像信息
rbd snap ls image 查看镜像快照
rbd snap create 镜像名字 --snap 快照名
rbd snap rollback 镜像名字 --snap 快照名
rbd snap protect 镜像名字 --snap 快照名字   保护快照
rbd clone 镜像名字 --snap  快照名字 新镜像名字 --image-feature layering
ceph-deploy mds create node4
