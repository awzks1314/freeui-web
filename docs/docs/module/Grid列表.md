#### 引用组件

**全局引用**

在`app.json`的`usingComponents`里引用

**单页引用**

在`对应page.json`的`usingComponents`里引用
```json
	{
	  "navigationBarTitleText":"FreeUI组件库",
	  "usingComponents": {
		"free-list-grid":"/components/module/free-list-grid/free-list-grid"
	  }
	}
```

#### 代码演示

**默认用法**

```html
	<free-list-grid 
		list="{{gridList}}" 
		col="{{col}}" 
		row="{{row}}"
		border="{{border}}"
		radius="{{radius}}"
		isSwiper="{{isSwiper}}"
		swiperHeight="{{swiperHeight}}"
		bind:click='onClick'
	></free-list-grid>
```

**几行几列**

`col`表示列数,默认`4`；`row`表示列数,默认`2`；`list`表示list数组
```html
	  <free-list-grid list="{{gridList}}" col="4" row="3"></free-list-grid>
```

**边框**

`border`表示边框，默认为false
```html
	  <free-list-grid list="{{gridList}}" border></free-list-grid>
	  <free-list-grid list="{{gridList}}" ></free-list-grid>
```

**图片大小、圆角**

`width`表示默认图片宽度,默认`60`rpx；`height`表示默认图片高度,默认`60rpx`；`radius`表示图片圆角，默认`10`rpx；`list`数组里定义图片宽高
<br>
如果你不想在list里面定义图片的宽高，可以使用默认宽高
```html
	  <free-list-grid list="{{gridList}}" radius="500" height="100" width="100"></free-list-grid>
```

**可滑动金刚区**

`isSwiper`表示是否可滑动，默认为`false`；`swiperHeight`为滑动容器的高度，默认为`400rpx`，需在可滑动`isSwiper==true`下使用
```html
	  <free-list-grid list="{{gridList}}" ></free-list-grid>
	  <free-list-grid list="{{gridList}}" isSwiper></free-list-grid>
	  <free-list-grid list="{{gridList}}" isSwiper swiperHeight="400"></free-list-grid>
```
**Props**

| 参数     | 说明                                                   | 类型          | 默认值      | 可选值 |
| -------- | ------------------------------------------------------ | ------------- | ----------- | ------ |
| list   | 数组 = [{name：名字 number：角标 image：图片 width：图片宽 height：图片高 color：角标背景}] | Array        | []      | -      |
| col   | 列数                                               | [Number,String]        | 4      | -      |
| row   | 行数                                               | [Number,String]        | 2      | -      |
| border      | 边框                         | Boolean       | false           | -      |
| bgColor   |  背景色                | String         | -#fff          | -      |
| width     | 图片默认宽，rpx                                 | String        | 60 | - |
| height     | 图片默认高，rpx             | String        | 60 | - |
| radius     | 图片圆角                                   | [Number,String]        | 10 |- |
| isSwiper    | 是否可滑动，可做金刚区                                    | String        | 28rpx 30rpx      |       |
| swiperHeight   | 滑动容器的高度，需搭配isSwiper使用| [Number,String]       | 400     | -     |
                     |             

**Events**

| 事件名称     | 说明                                                   | 回调参数      |
| -------- | ------------------------------------------------------ | ------------- |
| click      | 点击触发                          | {index:index索引}  |                

#### 预览

打开微信，扫码快速预览

<div align="left"><image src="https://z3.ax1x.com/2021/06/01/2nN0yt.jpg" width="200" height="200"> </image></div>
