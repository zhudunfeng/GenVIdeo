# GenVIdeo
一种基于python编写的视频自动生成程序<br>

项目安装<br/>
- 创建虚拟环境
```shell
python -m venv venv
```
- 切换到虚拟环境
```shell
./venv/Scripts/activate
```
- 安装依赖
```shell
python install -r requirements.txt
```
如果个人修改了依赖版本，可以冻结自己的依赖
```shell
pip freeze > requirements.txt
```

- 数据库可以根据DataBase.py自己进行配置

<h2>一、已经实现的功能：</h2>
<h3>1、文字转视频</h3>
 任意输入或者利用爬虫爬取一段文字语料，首先将其生成音频，然后将这段音频生成视频并添加字幕。<br>
 音频中可加入各种声效，视频可换任意背景图<br>
<h3>2、音频转视频</h3>
输入一段音频，语音识别生成文字，然后生成对应的字幕视频。<br>
<h3>3、快速生成动态排名数据可视化视频</h3>
运用movie中的模块将matplotlib画出的图表变成动画，效果如下链接所示：
(https://github.com/qihao123/GenVIdeo/video_example/Historical_ranking_data_visualization_example.mp4)
<h2>二、接下来想要实现的功能</h2>
<h3>功能1：新闻视频快速生成</h3>
对于新发生的新闻内容进行爬取，然后将文字转语音，根据图片生成视频，并添加字幕.（新闻类型可选）
<h3>功能2：房产/汽车/商品，图片+介绍文字进行视频生成+精准投放</h3>
根据商品图片&文字描述，生成视频简介。精准投放需投放平台支持，提供相关数据。
<h3>功能3：音视频分离，音频分离</h3>
目前支持分离鼓声、人声、伴奏、钢琴声、其他声音。详情见spleeter库
<h3>功能4：视频风格转移</h3>
爬取或自己上传视频，逐帧进行图像风格转移并拼接，整体转漫画风，梵高风等
<h3>功能5：统计排名类视频制作</h3>
爬取相关统计年鉴数据批量制作统计类视频。之前做的效果不是很好，需要进行改版。
<h3>功能6：视频分发</h3>
接入不同平台的视频上传接口，将自动制作的视频进行分发上传。（平台可定制开发）
<h3>功能七：视频播放数据分析</h3>
将视频播放数据进行定时采集，分析视频热度情况，并进行针对性制作。
<br>
<h2>三、平台相关</h2>
<h3>1、web端</h3>
 目前有在规划该项目的落地方案，目前考虑的就是编写web端应用，在web端实现上述功能。<br>
 业务上的东西我也是一知半解的。故需要志同道合的小伙伴一起来完成这个事情。<br>
 如果有感兴趣的产品经理、前端工程师、后端工程师、音视频处理工程师、新媒体运营等，只要感兴趣都可以一起聊聊。<br>
 ps：最好先发个邮件介绍一下你自己哦！<br>
<h3>2、手机端/小程序</h3>
手机端，我规划是主要用于相关数据与关键指标的展示。
<h2>四、目前需要的python依赖：</h2>
moviepy,pymysql,json,jieba,urllib,librosa,uuid,datatime,baidu-aip,spleeter
moviepy运行前还需要安装imagemagick的应用程序，在ImageMagic文件夹下，moviepy安装还需要修改一些配置，请自行查阅相关方法<br>
有问题请提issue，或发邮件至qihoo2017@gmail.com<br>
ps:发送邮件请注明来意。<br>
<br><br>


