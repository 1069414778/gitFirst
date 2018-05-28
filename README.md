# walkerHJ.github
####  javaScript弹出层<br/> #
![](JqPopup/1.jpg)
![](JqPopup/2.jpg)
![](JqPopup/3.jpg)
![](JqPopup/4.jpg)
![](JqPopup/5.jpg)
####  调用方式：<br/> #
<pre>
  <code>
    $('.item-1').click(function(){
		$(this).popup({
			'width':'500px',
			'height':'250px',
			'popup_Text':'title-test',
			'openEle_center_select':0,//0为text  1为html
			'openEle_center':'测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容',//为0时内容
			'openEle_center_tag':'<span>我是一段自定义html</span><br/><input type="text">',//为1时内容
			'masking':true,//是否需要蒙版
			'location':'https://www.baidu.com/',
			'yes':function(){
				$(this).msgopen({
					'text':'成功后回调函数',
					'time':2,
				})
			},
			'no':function(){
				$(this).msgopen({
					'text':'失败后回调函数',
					'time':2,
				})
			},
		});
	})
	$('.item-2').click(function(){
		$(this).msgopen({
			'text':'测试内容',
			'time':2,
		})
	})
	$('.item-3').click(function(){
		$(this).confirm({
			'popup_Text':'信息',
			'openEle_center':'你确定要删除吗~',
			'masking':true,//是否需要蒙版
		})
	})
  </code>
</pre>
