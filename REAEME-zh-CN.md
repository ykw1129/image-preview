简体中文 | [English](./README.md)

# image-preview(流畅 & 舒适)
一个前端图片预览插件 绝佳的手势体验，如果有使用到，请给我一颗`star`，阿里嘎多😁
### 特点:
1. 支持绝大部分的手势操作.
2. 旋转&缩放图片.
### 使用方法:
#### 下载:
* 克隆本项目，执行npm run build 命令 然后在`release/ts` 项目下找到`ImagePreview-prd.js`就可以直接使用了。
* 或者直接下载github上的`release/ts/ImagePreview-prd.js` 。
* 如果你的项目使用了模块管理系统：
* `release/image-preview`目录下为不同的模块系统生成了不同的代码，你可以选择一个适合你的项目下载下来。
#### 实例
[点击这里](http://122.51.15.11:9999) . 
#### 代码:
html:
```html
  <div class="imageWraper">
    <img data-src="/images/IMG_0512.JPG" src="/images/IMG_0512.JPG">
    <img data-src="/images/main_body3.png" src="/images/main_body3.png">
  </div>
```
javascript:
``` javascript
//just
let imgObj = new ImagePreview({
  selector:`.imageWraper img`
})
//or mvvm project

let imgObj =  new ImagePreview({
  curImg:'imgsrc',
  imgs:[
    'imgsrc',
    'imgsrc',
    'imgsrc'
  ]
})
//then show n-th picture,use
imgObj.show(n);
// distroy instance.  remove HTML generated by this ImagePreview instance
// for better performance, then you can set imgObj = null;
imgObj.distory();

```
### 交流
你可以加入这个qq群977121370与我交流.
