## 前言

欢迎来到微信小程序书店SpringBoot项目！本项目旨在为广大开发者提供一个微信小程序书店的实战案例，让大家更好地了解和掌握微信小程序与SpringBoot技术的整合开发。以下是对本项目的详细介绍。

## 内容介绍

本项目是一个基于微信小程序的书店系统，用户可以在微信小程序端浏览图书、查看图书详情、加入购物车、下单购买等。后端采用SpringBoot框架，实现用户、图书、订单等模块的管理。通过本项目，您可以学习到微信小程序与SpringBoot的实战开发技巧，提高自己的编程能力。

## 技术介绍

- **语言：** Java
- **使用框架：** Spring、SpringMVC、MyBatis、微信小程序
- **前端技术：** JS、Vue、CSS3、Uniapp
- **开发工具：** IDEA/Eclipse、Uniapp
- **数据库：** MySQL 5.7/8.0
- **数据库管理工具：** phpstudy/Navicat
- **JDK版本：** jdk1.8
- **Maven：** apache-maven 3.8.1-bin
- **前端环境：** Node.Js 12\14\16

## 核心代码

以下是本项目中的一个核心代码片段，展示了如何使用SpringMVC接收前端传来的参数，并返回图书列表。

```java
@RestController
@RequestMapping("/api/book")
public class BookController {

    @Autowired
    private BookService bookService;

    @GetMapping("/list")
    public ResponseEntity<List<Book>> list(@RequestParam("categoryId") Integer categoryId,
                                          @RequestParam("page") Integer page,
                                          @RequestParam("pageSize") Integer pageSize) {
        Page<Book> pageInfo = bookService.listBooks(categoryId, page, pageSize);
        return ResponseEntity.ok(pageInfo.getList());
    }
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img12.360buyimg.com/ddimg/jfs/t1/345418/30/3067/120124/68c59d07Fd67467bb/e503562a49e2899a.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/342513/23/3105/14194/68c59cdeF3f7c6c59/6d5812b2c6207c20.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/349330/17/3047/61260/68c59cdfFe1a0d2a0/62ba0ea6c002ef96.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/341774/19/2440/61760/68c59cdfF729b1157/9d2139c9ef4f4585.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/344815/19/2966/37859/68c59cdfF50037f55/71fe11caf4a35b93.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/334494/40/12887/57580/68c59cdfFc8f653ac/c9aa63001b7fa685.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/337525/19/10216/13041/68c59cdfF0966b2b3/54e4ecc6a26365bc.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/339814/19/10213/65305/68c59ce0Fbe1776b5/2ac1eeb6be51a91d.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/325535/17/19751/29775/68c59ce0F19ec8e7b/02497f950886c4e0.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/326587/21/19663/64387/68c59ce0Fef7b0c07/34a1e787a7c2df27.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
