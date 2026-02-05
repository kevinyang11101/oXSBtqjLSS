# 前言

欢迎来到本项目的Gitee页面！这是一个基于SpringBoot的房屋交易平台，是我毕业设计阶段的实践项目。在此，我分享这个项目的源码、文档报告以及部分代码讲解，希望能对有需要的朋友提供一些帮助。

# 内容介绍

本项目是一个房屋交易平台，主要实现了房屋信息发布、浏览、搜索、预约看房等功能。用户可以根据地区、价格、户型等条件筛选房源，同时可以查看房源的详细信息并预约看房。此外，平台还为房东和租客提供了交流的渠道，便于双方沟通。

# 技术介绍

## 语言：Java

## 使用框架：Spring Boot

## 前端技术：JS、Vue、css3

## 开发工具：IDEA/Eclipse

## 数据库：MySQL 5.7/8.0

## 数据库管理工具：phpstudy/Navicat

## JDK版本：jdk1.8

## Maven：apache-maven 3.8.1-bin

## 前端环境：Node.Js 12\14\16

# 核心代码

以下是项目中的一部分核心代码，用于展示房源列表：

```java
// HouseController.java
@GetMapping("/houses")
public String houses(Model model) {
    List<House> houses = houseService.findAll();
    model.addAttribute("houses", houses);
    return "houses";
}
```

```html
<!-- houses.html -->
<div v-for="house in houses" :key="house.id">
    <div class="house-item">
        <img :src="house.imgUrl" alt="">
        <div class="house-info">
            <h3>{{ house.title }}</h3>
            <p>{{ house.address }}</p>
            <p>{{ house.price }}/月</p>
        </div>
    </div>
</div>
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img12.360buyimg.com/ddimg/jfs/t1/326705/27/4481/130592/689de379F69ff521b/c9b0b00c70fdb2f8.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/290635/8/25431/66067/689de363Ffd2c3989/3a9472727b8b072a.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/311426/36/26180/38611/689de365F378c0760/112ad902a9026cc0.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/317036/15/23759/81573/689de363F6494eea4/a5dfa4cb58d6b18f.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/311823/18/26507/40229/689de366F805b597a/801001cea0eca646.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/291415/11/21735/37277/689de366F4cc5c7a6/06f1f9361be82b49.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/293108/37/23312/37956/689de367F239e3ab8/538c51c331c04a39.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/323798/4/4481/40757/689de367F239d4845/1c8222910f6b55c4.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/312789/11/26770/30619/689de368F34649603/daab3fcbfe706279.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/293903/10/12106/60731/689de368F5b8c7eea/196cf30b0f422265.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
