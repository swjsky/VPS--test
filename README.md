1.老鬼大佬的SuperBench测试脚本

这个脚本是在基于秋水大佬脚本的基础上，加入了独服通电时间，服务器虚拟化架构等内容

特点：

改进了显示的模式，基本参数添加了颜色，方面区分与查找。

I/O测试，更改了原来默认的测试的内容，采用小文件，中等文件，大文件，分别测试IO性能，然后取平均值。

速度测试替换成了 Superspeed 里面的测试，第一个默认节点是，Speedtest 默认，其他分别测试到中国电信，联通，移动，各三个不同地区的速度。
wget -qO- --no-check-certificate https://raw.githubusercontent.com/oooldking/script/master/superbench.sh | bash
#或者
curl -Lso- -no-check-certificate https://raw.githubusercontent.com/oooldking/script/master/superbench.sh | bash

Zbench
脚本由漏水和kirito，基于Oldking大佬 的 SuperBench，然后加入Ping以及路由测试的功能，还能生成测评报告，分享给其他人查看测评数据
#中文版
wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/ZBench/master/ZBench-CN.sh && bash ZBench-CN.sh
#英文版
wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/ZBench/master/ZBench.sh && bash ZBench.sh

LemonBench
LemonBench工具(别名LBench、柠檬Bench)，是一款针对Linux服务器设计的服务器性能测试工具。通过综合测试，可以快速评估服务器的综合性能，为使用者提供服务器硬件配置信息
curl -fsSL https://ilemonrain.com/download/shell/LemonBench.sh | bash
#或者
wget -qO- https://ilemonrain.com/download/shell/LemonBench.sh | bash

UnixBench测试脚本
UnixBench是一个类unix系（Unix，BSD，Linux）统下的性能测试工具，一个开源工具，被广泛用与测试linux系统主机的性能。Unixbench的主要测试项目有：系统调用、读写、进程、图形化测试、2D、3D、管道、运算、C库等系统基准性能提供测试数据。
wget --no-check-certificate https://github.com/teddysun/across/raw/master/unixbench.sh
chmod +x unixbench.sh
./unixbench.sh

回程路由测试
从你的 Linux(X86/ARM)/Mac/BSD 系统环境下发起 traceroute 请求，附带链路可视化，兼容性更好，支持 JSON 格式
下载
https://cdn.ipip.net/17mon/besttrace4linux.zip
#解压
unzip besttrace4linux.zip
#使用
./besttrace -q 1 这里是目标IP
