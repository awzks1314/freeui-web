#### 引用组件

**全局引用**

在`app.json`的`usingComponents`里引用

**单页引用**

在`对应page.json`的`usingComponents`里引用
```json
	{
	  "navigationBarTitleText":"FreeUI组件库",
	  "usingComponents": {
		"free-list":"/components/module/free-list/free-list"
	  }
	}
```

#### 代码演示

**默认用法**

```html
	<free-list 
	    arrow="true" 
	    icon="home" 
	    title="默认标题"
	    >
	</free-list>
```

**右侧箭头**

`arrow`属性用来表示右侧有无箭头,默认`false`
```html
	<free-list arrow title="有箭头"></free-list>
	<free-list arrow="{{false}}"   title="无箭头"></free-list>
```

**左侧图标/图片**

`icon`表示左侧图标；`iconColor`表示图标颜色；`image`表示是图片还是icon，默认为`false`
```html
	<free-list icon="home" title="默认标题"></free-list>
	<free-list icon="home" iconColor="#0081ef" title="默认标题"></free-list>
	<free-list icon="/static/images/my/dog.jpg" image title="默认标题"></free-list>
```

**大小**

`size`属性用来表示标题字体大小、图标大小，默认28rpx
```html
	<free-list  title="默认标题"></free-list>
	<free-list  title="默认标题" size="32"></free-list>
```
**Props**

| 参数     | 说明                                                   | 类型          | 默认值      | 可选值 |
| -------- | ------------------------------------------------------ | ------------- | ----------- | ------ |
| title   | 标题名称                                               | String        | -      | -      |
| color   | 标题颜色                                               | String        | #333      | -      |
| sub   | 副标题                                               | String        | -      | -      |
| arrow      | 右侧箭头                         | Boolean       | false           | -      |
| icon   |  图标                | String         | -           | -      |
| iconColor     | 图标颜色                                   | String        | - | - |
| image     | false表示内置图标，true表示引用图片            | Boolean        | false | - |
| size     | 图标及标题大小，单位rpx                                   | Number        | 28 | - |
| padding    | 列表内边距                                    | String        | 28rpx 30rpx      |       |
| bgcolor   | 背景颜色| String        | #fff      | -     |
| last   | 最后一条数据隐藏底部线条                       | Boolean        | false      |      |
| lineLeft   | 左边线条收缩                       | Boolean        | true      |      |
| lineRight   | 右边线条收缩                       | Boolean        | true      |      |

**Slots**

| 名称     | 说明                                                   |
| -------- | ------------------------------------------------------ | 
| default      | 右侧自定义内容展示                          |             

**Events**

| 事件名称     | 说明                                                   | 回调参数      |
| -------- | ------------------------------------------------------ | ------------- |
| click      | 时间点击时触发                          | -  |                

#### 预览

打开微信，扫码快速预览

<div align="left"><image src="https://z3.ax1x.com/2021/06/01/2nN0yt.jpg" width="200" height="200"> </image></div>
