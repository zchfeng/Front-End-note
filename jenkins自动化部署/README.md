# Jenkins自动化部署

## 安装
### 1、下载 https://www.jenkins.io/download/  （这是在Windows直接下载安装包）
![](./imgs/jenkins1.png)
一直Next进行  

![](./imgs/jenkins2.png)

### 2、注册 https://www.jenkins.io/zh/doc/book/installing/#unlocking-jenkins （密码安装截图提示路径去找相应文件）

![](./imgs/jenkins3.png)
![](./imgs/jenkins4.png) 

设置登录账号、密码、邮箱 

![](./imgs/jenkins5.png)

## 部署
  ### 1.安装GitLab Authentication plugin，GitLab Plugin，Publish Over SSH，Credentials plugin 插件 
  ![](./imgs/jenkins6.png)
  ![](./imgs/jenkins7.png)

  ### 2.添加凭据 
  ![](./imgs/jenkins8.png)
  ![](./imgs/jenkins9.png)
  ![](./imgs/jenkins10.png)
  ![](./imgs/jenkins11.png)

  **注：SSH的密钥是id_rsa文件的key**
  ![](./imgs/jenkins12.png)

  添加脚本语言（避免执行shell报错）
  ![](./imgs/jenkins13.png)

  ### 3、添加项目
  ![](./imgs/jenkins14.png)
  ![](./imgs/jenkins15.png)
  ![](./imgs/jenkins16.png)
  ![](./imgs/jenkins17.png)
  ![](./imgs/jenkins18.png)
  ![](./imgs/jenkins19.png)

  保存

  ## 4、下载nginx 

  ### 4.1 http://nginx.org/en/download.html（我这里是下载Windows版本）
  ![](./imgs/jenkins20.png)

  ### 4.2 解压后运行nginx
  直接在文件夹双击nginx.exe或者用cmd cd到文件夹运行输入命令 nginx.exe 或者 start nginx ，回车即可完成启动

  ![](./imgs/jenkins21.png)

  ### 4.3 设置nginx server
  ![](./imgs/jenkins22.png)

  打开http://localhost:7777/