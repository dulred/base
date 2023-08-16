#### 搭建gitlab-ci-cd过程
>  1.购买阿里云服务器
> 2.在服务器上安装gitlab-ce
> 3.在服务器上安装gitlab-runner
> 4.将本地项目推送到gitlab,触发自动部署

1.配置apt镜像源

2.更新镜像源sudo apt-get update 

3.sudo apt-get install curl openssh-server ca-certificates postfix 

postfix 软件安装后会弹出一个”Postfix Configuration”向导，直接选`No configuration`不进行配置（本地环境不实用）

4.wget --content-disposition https://packages.gitlab.com/gitlab/gitlab-ce/packages/ubuntu/jammy/gitlab-ce_15.8.3-ce.0_amd64.deb/download.deb

> gitlab官方下载 站 https://packages.gitlab.com/gitlab/gitlab-ce/packages/ubuntu/jammy/gitlab-ce_15.8.3-ce.0_amd64.deb

5.安装 sudo dpkg -i gitlab-ce_15.8.3-ce.0_amd64.deb 

6.修改外部url和reconfigure

7.修改密码



_参考_

[Ubuntu Server 22.04 安装 Gitlab-ce](https://kiraster.github.io/posts/ed7bc2e7.html#%E4%B8%8B%E8%BD%BD%E5%92%8C%E5%AE%89%E8%A3%85gitlab-ce-15-8-3)