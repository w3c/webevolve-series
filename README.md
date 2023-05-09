# 搭建jekyll会议页面

## 复制代码

1. 从模板复制一份代码 https://github.com/w3c-beihang/meeting-template/fork 到目标仓库
2. 修改内容后，启动 GitHub Pages

## 代码结构

- index.html 首页
- cfp.html 内容页1
- sponsorship.html 内容页2
- _data
-    -> pages.yml 导航配置页
- _includes
-    -> sponsors.html 页面通用区块
- _layouts
-    -> default.html 所有页面通用模板
- script.js JavaScript脚本
- style.css 页面样式文件

## 本地安装运行jekyll -- 用于看效果

```
gem install jekyll
jekyll new my-awesome-site
cd my-awesome-site
jekyll serve
# => Now browse to http://localhost:4000
```

## 在GitHub 配置服务器
1. 确保项目是public的repo
2. 打开GitHub pages 开关，一般在开关在 https://github.com/xxx/xxx/settings/pages. 在【Branch】下拉框选择'main'分支，点击【save】按钮即可。
3. 在新项目里删掉这个README.md、.gitignore文件，因为所有根目录的文件都可以访问。这些文件不需要。
4. 点击对应地址看效果，如 https://w3c-beihang.github.io/meeting-template/