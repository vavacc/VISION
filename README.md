# VISION
全球引领主流搬运工
教程开始：
1.申请SSL证书：

申请前请检查是否开启了防火墙（UFW），如果开启了请关闭，关闭命令：sudo ufw disable

apt update -y    #更新系统

apt install -y curl    #安装curl

apt install -y socat    #安装socat

curl https://get.acme.sh | sh    #安装Acme脚本

~/.acme.sh/acme.sh --register-account -m vsva911@outlook.com    #设置SSL申请邮箱，xxxxxx@xxx.com更换为自己的邮箱

~/.acme.sh/acme.sh --issue -d coc.soscc.eu.org --standalone    #申请SSL，xxxx.xxx更换为自己的域名

~/.acme.sh/acme.sh --installcert -d coc.soscc.eu.org  --key-file /root/private.key --fullchain-file /root/cert.crt    #安装证书文件到root目录下，xxxx.xxx更换为自己的域名

公钥文件路径：        /root/cert.crt

密钥文件路径：        /root/private.key

SSL证书申请完成

2.安装X-UI面板
bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)


安装X-UI面板
bash <(curl -Ls https://raw.githubusercontent.com/vavacc/SOLO-X-UI/main/install.sh)

备用
https://raw.githubusercontent.com/vavacc/SOLO-X-UI/main/install.sh
