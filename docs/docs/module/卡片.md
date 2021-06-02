#### 引用组件

**全局引用**

在`app.json`的`usingComponents`里引用

**单页引用**

在`对应page.json`的`usingComponents`里引用
```json
	{
	  "navigationBarTitleText":"FreeUI组件库",
	  "usingComponents": {
		"free-tag":"/components/basic/free-tag/free-tag"
	  }
	}
```

#### 代码演示

**默认用法**

```html
	<free-tag 
	    type="{{type}}"
	    size="{{size}}"
	    radius="{{radius}}" 
	    effect="{{effect}}"
	    icon="{{icon}}"
	    iconColor="{{iconColor}}"
	  >默认标签</free-tag>
```

**标签颜色**

`type`属性用来表示颜色，默认`blue`
```html
	<free-tag type="blue">默认标签</free-tag>
```

**标签大小**

`size`属性用来表示标签大小
```html
	<free-tag >默认标签</free-tag>
	<free-tag size="sm">默认标签</free-tag>
```
**标签圆角**

`radius`属性用来表示标签圆角，默认`5000rpx`,圆角
```html
	<free-tag >默认标签</free-tag>
	<free-tag radius="10rpx">默认标签</free-tag>
	<free-tag radius="30rpx">默认标签</free-tag>
```

**标签主题**

`effect`属性用来表示标签主题，默认`dark`，可选`dark`/`light`/`plain`
```html
	<free-tag effect="dark">默认标签</free-tag>
	<free-tag effect="light">默认标签</free-tag>
	<free-tag effect="plain">默认标签</free-tag>
```

**标签图标**

`icon`属性用来给标签加图标，`iconColor`表示图标的颜色，可选图标为内置图标
```html
	<free-tag icon="home">默认标签</free-tag>
	<free-tag icon="home" iconColor="#000">默认标签</free-tag>
```

**Props**

| 参数     | 说明                                                   | 类型          | 默认值      | 可选值 |
| -------- | ------------------------------------------------------ | ------------- | ----------- | ------ |
| type   | 标签的颜色                                               | String        | -      | 见下表      |
| radius      | 标签圆角                                           | String        | 5000rpx           | -      |
| padding   |  标签内边距                | String         | -           | -      |
| shadow     | 标签阴影                                   | Boolean        | true | - |
| size    | 标签大小                                              | String        | -      | sm      |
| effect   | 标签主题| String        | dark      | dark/light/plain      |
| icon   | 图标名字                                               | String        | -      | 内置icon图标      |
| iconColor   | 图标颜色                                               | String        | #fff      | -      |

**type的取值**

| 参数         | 默认值                                                      | 值                                                      |
| ------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 嫣红  | red | #e54d42 |
| 桔橙    | orange | #f37b1d |
| 明黄   | yellow | #fbbd08 |
| 橄榄     | olive | #8dc63f |
| 森绿    | green | #39b54a |
| 天青          | cyan | #1cbbb4 |
| 海蓝       | blue | #0081ff |
| 姹紫       | purple | #6739b6 |
| 木槿         | mauve | #9c26b0 |
| 桃粉        | pink | #e03997 |
| 棕褐     | brown | #a5673f |
| 玄灰    | grey | #8799a3 |
| 草灰  | gray | #aaaaaa |
| 墨黑 | black | #333333 |
| 雅白 | white | #ffffff |

#### 预览

打开微信，扫码快速预览

<div align="left"><image src="https://z3.ax1x.com/2021/06/01/2nN0yt.jpg" width="200" height="200"> </image></div>
