# draggable-vue-uploade

<div align="center">

简体中文 | [English](./README.en.md)

</div>

一个简单的图片上传组件, 支持图片列表拖拽排序。

如果项目对你有所帮助, 欢迎star!

**支持 Vue 3**

## 安装
```
npm i draggable-vue-uploader
```

## 使用
```
import DraggableUploader from 'draggable-vue-uploader';
import 'draggable-vue-uploader/dist/style.css'

createApp(App).use(DraggableUploader).mount('#app')

```

## 例子
[demo](https://hello7cat.com/draggable-vue-uploader/)

## 运行demo

cd example

npm run i

npm run dev

## 文档

### 传参
|参数名|描述|类型|默认值|
|---|---|---|---|
|action|上传的URL|`string`|`-`|
|fileList|文件列表|`FileItem[]`|`-`|
|maximum|列表最大上传数|`number`|`10`|
|before-upload|上传文件前触发|`(file: File) => boolean\| Promise`|`-`|
### 事件
|事件名|描述|参数|
|---|---|---|
|change|上传的文件状态发生改变时触发|fileList: `FileItem[]`<br>fileItem: `fileItem`|
|progress|上传文件进度条|fileItem: `fileItem`<br>progress: `progress`|
|success|上传成功|fileItem: `fileItem`<br>result: `result`|
|error|上传失败时触发|fileItem: `FileItem`<br>error: `error`|

## 待办

- [x] 基础功能
- [x] 图片预览
- [x] 打包发布
- [ ] 动画

