# level-2

本关先提交正常弹窗脚本测试：

![image](assets/image-20260324200815-rejp6d0.png)

发现在input标签中，作为value的属性值以双引号闭合，那么绕过思路就是闭合该标签以及双引号

**payload:">alert(1)**
