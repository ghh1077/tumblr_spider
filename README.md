#修改自大佬的脚本

原脚本由于api显示每个username只能爬第一页图片，修改为爬去所有图片

修改获取照片尺寸由520变为1280

增加超时检测，tumbler国内访问容易超时卡死
    默认为30s，网络环境好可在34行减少数值，反之亦然

修改只获取图片，小视频质量一般哈，有需求去爬视频网站好了
    需要获取小视频在16行删除type=photo&即可

没有验证任务结束，出现报错即完成

使用方式不变C:\Users\liguo\Documents\GitHub\tumblr_spider

# python3 tumblr多线程爬虫
给定 tumblr 用户的 username ，下载图片以及视频资源。  
声明一下:这是一个正经的爬虫，所爬取的资源跟你填入的 username 有关系，请勿随意开车。  
另外，由于tumblr被墙，请使用代理爬取。

# 资源存储
>图片存放在tumblr.py所在文件夹下的'/etc/img'中，修改imgDir即可修改文件存放位置。  
>视频存放在tumblr.py所在文件夹下的'/etc/mp4'中，修改videoDir即可修改文件存放位置。

# 运行
>python tumblr.py username1[,username2,username3...]

# import
>import tumblr  
>tumblr.tumblr_id('username1,username2,username3...')
原脚本地址
https://github.com/yl-L/tumblr_spider
