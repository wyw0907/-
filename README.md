# -
基于pcDuino开发板，linux，AndroidApp，Web等平台，使用c/c++创建的网络视频监控系统

本视频监控系统通过网络传输视频数据，只要有网络连接，用户就可以远程观看视频监控画面。系统包括视频监控端，服务器和客户端。视频监控端负责采集图像，并将图像数据发送到服务器，摄像头可以在本地缓存一定时间的图像。服务器负责汇聚、转发、分发各个前端监控点的视频码流，并完成系统的管理控制功能。用户通过客户端查看视频图像，设置摄像头参数，和其他高级功能配置。


视频监控系统
	监控端
		图像采集
			v4l2摄像头驱动
			图像压缩
		服务器连接
			视频数据传输
			控制信息
		图像存储
		图像处理
			face++人脸识别
		云台
	服务器
		http服务器
			主页
			网页查看摄像头图像
			客户端连接API
				Get
				Post
		数据库
		tcp	自定协议
			云台控制
			监控端连接API
	客户端
		用户注册
		二维码扫描绑定摄像头
		从服务器获取视频图像
			实时图像
			历史图像
		摄像头参数设置
			分辨率
			帧率
			摄像头角度
