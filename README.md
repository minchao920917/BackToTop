回到顶部(兼容ie8)

![QQ截图20180409110932.png](https://i.loli.net/2018/04/09/5acada222f5da.png)


1、参数列表

	var options = {
			setting: { 
				startline:200, 			// 鼠标向下滚动距离，出现#topcontrol图标
				scrollto:100, 			// 它的值可以是整数，也可以是一个id标记。
				scrollduration:10000, 	// 滑动到的scrollto的速度，值越大越慢
				fadeduration:[100, 100]	//#topcontrol这个div的淡入淡出速度，第一个参数为淡入速度，第二个参数为淡出速度
			},
			controlHTML: '<a href="#top" class="top_stick"><img src="images/scroll-top.png" style="width:50px; height:50px" /></a>',//控制向上滑动的html源码
			controlattrs: {	//控制#topcontrol这个div距离右下角的像素距离	
				offsetx:100, 
				offsety:310
			},
			anchorkeyword: '#top',//滑动到的id标签
			state: {
				isvisible:false,  	//是否#topcontrol图标这个div为可见
				shouldvisible:false //是否#topcontrol图标这个div该出现
			}
		}

2、调用方法
	
	$(window).BackToTop(options);