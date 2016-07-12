---
layout: post
title: Audio音频标签的使用
category: 技术
tags: [tech]
keywords: html5
description: 学习了Audio标签的使用，记录一下。
---

### 标签描述

	html5增加的音频标签，可以在开始标签和结束标签之间放置文本内	容，这样老的浏览器就可以显示出不支持该标签的信息。
	
### source标签
	audio 元素允许多个 source 元素。source 元素可以链接不同的	音频文件。浏览器将使用第一个可识别的格式：	
	
	```
		<audio controls="controls">
 			 <source src="/i/song.ogg" type="audio/ogg">
 			 <source src="/i/song.mp3" type="audio/mpeg">
			Your browser does not support the audio element.
		</audio>
	```	
	
### 属性

	| 属性      | 值     | 描述 |
	| ------------- |:-------------:|:--------|
	| autoplay   | autoplay | 音频就绪后立即播放 |
	| control   | control | 显示播放器 |
	| loop   | loop | 每当音频结束时重新开始播放 |
	| preload | preload | 音频在页面加载时进行加载，预备播放 |
	| src   | url | 播放音频的路径|
	
### DOM Audio对象
	- 可以通过getElementById()来访问 <audio> 元素
		
		```
		var x = document.getElementById("myAudio");
		
		```
		
	- 可以通过使用createElement()方法来创建 <audio> 元素
		
		```
		var x = document.createElement("AUDIO");
		
		```	
		
	- Audio对象属性（常用）
	
		| 属性   | 描述 |
		| ------------- |:-------------:|
		| autoplay  | 设置或返回是否在加载完成后随即播放音频 |
		| controls  | 设置或返回音频是否应该显示控件|
		| currentSrc  | 返回当前音频的 URL |
		| currentTime  | 设置或返回音频中的当前播放位置（秒）|
		| defaultMuted  | 设置或返回音频默认是否静音 |
		| duration  | 返回音频的长度（以秒计） |
		| ended  | 返回音频的播放是否已结束 |
		| loop  | 设置或返回音频是否应在结束时再次播放 |
		| muted  | 设置或返回是否关闭声音 |
		| networkState  | 返回音频的当前网络状态 |
		| paused  | 设置或返回音频是否暂停 |
		| preload  | 设置或返回音频的 preload 属性的值 |
		| readyState  | 返回音频当前的就绪状态 |
		| src  | 设置或返回音频的 src 属性的值 |
		| volume  | 设置或返回音频的音量 |
		
	- Audio对象方法（常用）
	
		| 属性   | 描述 |
		| ------------- |:-------------:|
		| canPlayType()  | 检查浏览器是否能播放指定音频类型 |
		| fastSeek()  | 在音频播放器中指定播放时间|
		| getStartDate()  | 返回新的 Date 对象，表示当前时间线偏移量 |
		| load()  | 重新加载音频元素 |
		| play()  | 播放音频 |
		| pause()  | 暂停音频 |
	


		
		


