---
title: 'Hugo PaperMod主题中正确显示中文字数统计的方法'
date: "2024-01-21"
tags: ["hugo","tutorials"]
---
当配置完PaperMod主题后，发现文章在中文下显示的字数统计是错误的。  
发现Hugo本身有个配置[hascjklanguage](https://gohugo.io/getting-started/configuration/#hascjklanguage)是支持中文/日文/韩文内容显示，但默认状态下为false。因此只需在你的config.yml文件添加**hasCJKLanguage: true**，即可对文章中文进行统计，字数统计数值此时显示正常。

在config.yml 添加以下内容：
```yml
languageCode: "zh-cn" # 默认语言为中文
hasCJKLanguage: true # 自动检测内容中的中文/日文/韩文
```
