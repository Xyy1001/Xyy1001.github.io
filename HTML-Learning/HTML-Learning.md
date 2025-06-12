# Baisc Concept of HTML
![The Simple Structure of HTML](HTML-Learning\HTMLstruc.png)
![Let's visualise the structure of HTML](HTML-Learning\HTML-Visual.png)
可视化中，只有<body>部分内容（白色部分）才会在浏览器中被渲染并显示

# <!DOCTYPE html>声明
## <!DOCTYPE>声明有助于浏览器中正确显示网页。
网络上有很多不同的文件，如下载链接，或者网页转换等，如果能够正确声明HTML的版本，浏览器就能正确显示网页内容。
## 不同版本HTML声明
需要注意的是，不同版本的html声明细节是不同的，例如：
HTML5是
### <!DOCTYPE html>
HTML4.01是
### <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
### "http://www.w3.org/TR/html4/loose.dtd">
XHTML 1.0是
### <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
### "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
### 查看完整页面生命请查看官方文档：https://www.runoob.com/tags/tag-doctype.html
## 冷知识：doctype 声明是不区分大小写的，也就是说“html”可以是H\T\M\L任意大小写字母的排列组合，而DOCTYPE同理

# 中文编码-条件
目前在大部分浏览器中，直接输出中文会出现中文乱码的情况，这时候我们就需要在头部将字符声明为UTF-8或GBK。
也就是在index.html文件中的“<meta charset="utf-8"><!--整个网页使用的渲染格式-->”