
# 安装步骤:
1. 安装mysql, 修改当前目录下comm.properties的相关配置.  
2. 使用root用户运行如下的命令获取并安装

```bash
$ cd /data
$ git clone https://github.com/l7l1l0l/Tars.git --recursive
$ cd /data/Tars/deploy
$ python ./deploy.py all
```

# 安装要求:
1. 以root权限运行
1. 支持python 2.7
2. 网络正常
3. 若缺少以下软件 :gcc,gcc-c++,cmake,yasm,glibc-devel,flex,bison,ncurses-devel,zlib-devel,autoconf ,
会尝试安装，但可能会失败
4. Tars 默认的mysql配置为/usr/local/mysql/， 若你的环境不一致，请修改CMakeLists.txt(framework/tarscpp/CMakeLists.txt, framework/CMakeLists.txt) 在编译之前。 
6. 需要python 的requests包，若未安装，请使用"pip install requests"

## 修改CMakeLists.txt

