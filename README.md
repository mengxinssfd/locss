# locss
locss是一个辅助程序员编写样式的工具类css库；与tailwind库不同，主要是提供一些比较常用或者是成套的css样式以供使用，主要的css还是得自己写。


locss的lo来源于lodash，意为css中的lodash(长远目标)，减少css代码量。

## 安装方式
cdn方式引入
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/locss@1.0.2/dist/index.min.css">
```
npm
```shell
npm install locss
```

## 使用方式
html元素的class添加_和功能class，如果class中没有"_"，那么功能class不会生效。
## 功能
### 文字缩略
##### 5行以内缩略
ellipsis-1 - ellipsis-5
```html
<div class="_ ellipsis-1"></div>
```
##### 5行以外缩略
ellipsis-mul 加 另外的css上 line-clamp: 行数;
-webkit-line-clamp: 行数;
```html
<div class="_ ellipsis-1"></div>
```

### flex布局
#### 常用的flex居中布局
y轴居中
```html
<div class="_ flex-c"></div>
```
等于
```css
.flex-c {
    display: flex;
    align-items: center;
}
```
x轴居中
```html
<div class="_ flex j"></div>
```
等于
```css
.flex-c {
    display: flex;
    align-items: center;
}
```
xy轴居中
```html
<div class="_ flex-c-c"></div>
```
等于
```css
.flex-c {
    display: flex;
    align-items: center;
    justify-content: center;
}
```