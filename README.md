# UeditorClient

### 一、项目概述

1、ueditor 是百度的开源富文本编辑器，有多个版本，本项目采用的是 1.4.3.3 jsp 版

2、ueditor 并不是一个纯粹的由 html/js/css 组成的前端项目，它还包含后端代码，因为编辑器本身包含图片上传等功能，

这些功能只能由后端来完成，这也是为什么分为 jsp/php/asp/.net 多个版本的原因。如果只是一个纯粹的前端项目，只需要一个版本就可以了。

3、也就是说 ueditor 其实就是一个传统的 jsp/servlet 项目，其运行也需要 tomcat,jvm 等

4、随着前后端分离的流行，原本的 ueditor 项目有许多局限性

(1) 项目中已经很少直接使用 jsp/servlet　编程了，ueditor显然已经落后于时代

(2)　现在通常只需要 ueditor 前端的功能，后端功能（如保存图片）自己写

(3)　ueditor 后端功能本身就有许多缺点，如文件保存位置很难自定义等

5、再次声明： ueditor 本身是一个完整的包含前后端的项目，对于 UeditorClient 来说，只采用了其前段功能，

后端功能参照 UeditorServer


### 二、运行

1、mvn clean package

2、mvn tomcat7:run

3、http://127.0.0.1:8080/UeditorClient
