# 黑马 Mybatis 参数传递\_思考题

[思考题链接](https://www.bilibili.com/video/BV1Qf4y1T7Hx?p=59&share_source=copy_web)

-   时间点：19:28

# 问题描述

![Img](https://typora-1313573096.cos.ap-guangzhou.myqcloud.com/typora/202210181818537.png)
接口方法参数是 map 集合对象，map 基础加入的数据类型为 user，SQL 语句应该如何编写，即问好处如何填写。

# 解答

答案：填 `user.username 和 user.password `

运行结果
![Img](https://typora-1313573096.cos.ap-guangzhou.myqcloud.com/typora/202210181818957.png)

此外：

-   问题描述的图片的 `user.setUsername(password);` 填错了 set 方法。

-   `User user = mapper.select(map);` 的 user 应改为其它变量名
