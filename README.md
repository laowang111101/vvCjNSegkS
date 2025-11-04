# 前言

随着新冠疫情的全球爆发，居家办公已经成为新常态。为了适应这种变化，我们开发了这款疫情居家办公系统，旨在帮助企业和员工实现高效、便捷的远程办公。本项目使用Java语言和MySQL数据库，基于Spring Boot框架开发，前端采用JS、Vue和CSS3技术。下面，让我们一起来看看这个项目的详细介绍。

## 内容介绍

疫情居家办公系统是一款集办公管理、任务分配、进度跟踪等功能于一体的在线办公平台。通过该系统，企业可以方便地管理员工，分配工作任务，实时跟踪项目进度；员工可以在线提交工作成果，反馈问题，提高工作效率。此外，系统还提供了疫情动态、健康打卡等功能，助力企业疫情防控。

## 技术介绍

- 语言：Java
- 使用框架：Spring Boot
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven：apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是疫情居家办公系统中一个简单的用户登录功能的核心代码：

```java
// 登录控制器
@RestController
@RequestMapping("/login")
public class LoginController {

    @Autowired
    private UserService userService;

    // 用户登录
    @PostMapping("/auth")
    public ResponseEntity<?> login(@RequestBody User user) {
        User result = userService.findByUsernameAndPassword(user.getUsername(), user.getPassword());
        if (result != null) {
            // 登录成功，返回用户信息
            return ResponseEntity.ok(result);
        } else {
            // 登录失败，返回错误信息
            return ResponseEntity.status(HttpStatus.UNAUTHORIZED).body("用户名或密码错误");
        }
    }
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/290792/31/22237/164097/689e1144F93cc6619/9859f51940a4e65a.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/289416/14/27442/34497/689e1122F1ee73dab/ba3422923851f4e7.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/314511/22/26350/113311/689e1122Ff34d9347/2b7f3727c55504e1.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/327102/31/4640/44096/689e1123F436e8eb7/bfd01dcb21d22804.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/316148/8/26368/29654/689e1124Fb1be4879/0d9b14808ef5319c.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/315095/30/26500/30325/689e1125Fd483a739/fa4d72521fc9ad3c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/319288/26/24752/54071/689e1125F4f18e43a/518213e9c966e30c.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/313346/2/26252/34876/689e1126F75035170/feada1422562449b.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/286669/24/27149/53118/689e1126Fa3113a35/095899e124dd2d8a.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/328843/35/4721/26580/689e1127F18d3f15c/de57587c18eca5a9.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
