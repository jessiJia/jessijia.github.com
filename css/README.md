# jessijia.github.com
#hexo + github 建立blog,需要安装hexo和git，需要一个git库，并建立一个以username.github.com命名的代码库

#hexo 
##hexo 初始化
hexo init 

#hexo 常用命令
hexo new "postName" #新建文章
hexo new page "pageName" #新建页面
hexo generate #生成静态页面至public目录
hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）
hexo deploy #将.deploy目录部署到GitHub

#hexo 复合命令
hexo deploy -g
hexo server -g

#hexo 简写命令
hexo n == hexo new
hexo g == hexo generate
hexo s == hexo server
hexo d == hexo deploy

#对blog的设定在_config.yml

#部署到github
deploy:
  type: git
  repository: <git代码库地址>
  branch: master #默认master
  ##执行hexo deploy后生成.deploy_git文件夹
