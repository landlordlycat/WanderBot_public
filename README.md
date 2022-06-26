# WanderingBot
未来地球流浪者bot - 基于WeChaty, PaddleHub与彩云小梦的科幻机器人
本版本已归档，代码请查看：https://github.com/sunyuqian1997/Wander001-V2.1
项目官网：www.wander001.com 目前微信好友已加满，若想体验请加入discord英文版：https://discord.gg/3njPKQJ4V4

<img src="image\4.jpg" alt="bf"  />



一个身处未来，正在努力穿越地球的旅行者。 可以跟人类发送当前定位、照片和游记。
希望做成一个互联网艺术项目，成为参与者聊天列表里一位特殊的旅行者，给参与者带去一些期待和惊喜。

详细与流程请见AI Studio：https://aistudio.baidu.com/aistudio/projectdetail/1896705



<img src="image\5.png" alt="bf"  />

<img src="image\3.png" alt="bf"  />

<img src="image\2.jpg" alt="bf"  />

<img src="image\1.jpg" alt="bf"  />



## 实现流程

获取地理信息，如 [北京大学东门]

=》调用百度地图api地图检索功能，根据地点搜索获取gps坐标

http://lbsyun.baidu.com/index.php?title=webapi/guide/webservice-placeapi

=》调用百度地图api全景静态图功能，获取该坐标对应的街景图

http://lbsyun.baidu.com/index.php?title=viewstatic

=》调用PaddleHub风格迁移模型，迁移成未来风格

https://aistudio.baidu.com/aistudio/projectdetail/439779?channelType=0&channel=0

=》调用彩云小梦api，生成游记

[https://open.caiyunapp.com/%E5%BD%A9%E4%BA%91%E5%B0%8F%E6%A2%A6API](https://open.caiyunapp.com/彩云小梦API)

=》通过WeChaty返回消息给用户

https://wechaty.js.org/



### 版本&要求

使用Python 3.7.4

服务器搭建，以及WeChaty Token获取的部分请参考：

https://aistudio.baidu.com/aistudio/projectdetail/1836012

百度地图的api Token(ak)可通过在官网控制台创建应用获得

[http://lbsyun.baidu.com/index.php?title=%E9%A6%96%E9%A1%B5](http://lbsyun.baidu.com/index.php?title=首页)

彩云小梦的api Token需要通过邮件申请

[https://open.caiyunapp.com/%E5%BD%A9%E4%BA%91%E5%B0%8F%E6%A2%A6API](https://open.caiyunapp.com/彩云小梦API)




### 参考链接
阿里云+wechaty教程
https://aistudio.baidu.com/aistudio/projectdetail/1836012

wechaty例子
https://github.com/Lovely-Pig/paddlehub-wechaty

百度地图 全景静态图api
http://lbsyun.baidu.com/index.php?title=viewstatic
https://zhuanlan.zhihu.com/p/79627772

百度地图-地点检索
http://lbsyun.baidu.com/index.php?title=webapi/guide/webservice-placeapi



### 文件夹

地点获取图片：pictures
迁移完成：transfer_result
风格图：style_transfer
百度api相关脚本：baiduScript



<img src="realLogo.png" alt="bf"  />
