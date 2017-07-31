百度贴吧采集图片站程序

## 前言 ##
该程序是根据系统后台设置贴吧名称后，系统根据所设置的贴吧进行指定采集。

采集完成后的图片保存在本地服务器，并生产数据于前端展示。

系统根据所设置贴吧名称指定采集相关贴吧信息图片，指定贴吧前，先检查该贴吧是否正常开放，如被关闭的贴吧是无法正常采集的。

采集逻辑为：

1、采集贴吧列表；

2、采集列表中具体帖子内容图片。

## 程序简介 ##
程序使用Thinkphp5.0.10 为程序框架开发

前端使用AmazeUI 2.7.2 进行制作

程序目前实现根据指定贴吧进行采集，将采集后的图片存入本地服务器，通过后台管理已采集数据和设置采集贴吧名称。前端实现显示数据，搜索数据，分页，评论等效果。

## 采集设置 ##
使用windows或linux制作两个定时执行器执行下面两个页面即可

1、设置采集列表 `http://youhost/getlist`

2、设置采集内容 `http://youhost/getimg`

> 列表采集建议每小时执行一次，内容建议30-60秒执行一次。
> 默认设置为图片大于4张采集，楼层小于20采集，如果需要可以自行修改

## 一些细节 ##
如果发现采集停止，需要查看/runtime/log/下面的日志情况。

如有更新可以清空/runtime 目录下的所有文件。

由于贴吧中部分帖子为广告贴，但采集无法识别，所有当采集后可以通过删除进行处理。

## 作者 ##

风之翼灵

问题反馈
[https://www.fungj.com/works/baidu-post-bar-picture-acquisition-system.html](https://www.fungj.com/works/baidu-post-bar-picture-acquisition-system.html "https://www.fungj.com/works/baidu-post-bar-picture-acquisition-system.html")

[www.fungj.com](http://www.fungj.com "www.fungj.com")

该程序由风之翼灵开发，如有问题请到www.fungj.com提出来

程序于2017年7月24日开发，同月27日上线并发布R1版本。

程序持续更新中，处理BUG，完善采集，优化系统，新增功能。