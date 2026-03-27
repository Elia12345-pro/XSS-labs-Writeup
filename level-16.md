# level-16

这一关先审计源码

![image](assets/image-20260327105440-mwntw4b.png)

网页通过接收keyword参数值返回到后端进行过滤，strtolower是php的一个函数，会把传入的参数字母全部转化为小写，接下来可以发现这一关的过滤规则非常严格，甚至连空格都会被替换。

既然空格行不通，可以用%0a换行符替代，在浏览器解析时可以达到和空格一样的效果

‍

payload:?keyword=<img%0asrc=1%0aonerror=alert(1)>
