# 搭建jekyll会议页面

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
2. 打开GitHub pages 开关，一般在开关在 https://github.com/xxx/xxx/settings/pages
3. 在新项目里删掉这个README.md文件，因为所有根目录的文件都可以访问。这个文件不需要。