# level-6

本关尝试之前关卡的方法发现都被过滤了，此时我们审计源码

![image](assets/image-20260325211606-swn1ln2.png)

发现源码使用了php的str_replace函数进行过滤，这个函数有一个特点就是区分大小写，那么我们可以使用大小写进行绕过

payload:"><SCRIPT>alert(1)</SCRIPT>
