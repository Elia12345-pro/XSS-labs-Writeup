# level-12

这一关审计源码发现和上一关相似的套路

![image](assets/image-20260326191632-8vlqo2i.png)

对http报头参数user-agent没有进行过滤，同样是用burp进行抓包修改

‍

payload:" type="text" onmouseover="alert(1)
