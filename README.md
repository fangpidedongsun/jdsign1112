尽量不要用action跑， 否则github封号，如需要github action运行,请注册帐户后先复制或导入其它项目,等一周后再复制本脚本.

低调使用，不要fork！尽量第一时间同步更新脚本。防止失联请收藏gitee备份地址：https://gitee.com/xr2021/jdsign
复制仓库后可以用github action 运行 

Action 打开方式 setting--actions ......Actions permissions
.........Allow all actions...save 



docker 一键安装：

wget  https://gitee.com/xr2021/jd-shell/raw/v3/install_scripts/docker_install_jd.sh -O docker_install_jd.sh && chmod +x docker_install_jd.sh && bash docker_install_jd.sh

安装完成后输入docker设备地址如192.168.1.1:5678 用户名admin密码admin5678 添加cookie，可进入后扫码获得，自行设定各脚本运行时间即可。




青龙拉库命令:
ql repo https://ghproxy.com/https://github.com/hajiuhajiu/jdsign1112.git "jd_|jx_|gua_|jddj_|getJDCookie" "activity|backUp" "^jd[^_]|USER|utils|function|ql"

定时规则0 */4 * * *

一、青龙运行python脚本缺少requests模块，请按以下方式安装：
1、进入青龙容器：docker exec -it qinglong /bin/sh
2、安装requests模块
pip3 install requests
3、安装完成，退出容器
exit

二、青龙安装nodejs模块方法：
1、进入青龙容器：
docker exec -it qinglong /bin/sh
2、进入/ql/scripts目录
cd scripts
4、安装png-js模块
npm install -g png-js
安装jsdom模块
npm install -g jsdom
5、安装完成，退出容器
exit


