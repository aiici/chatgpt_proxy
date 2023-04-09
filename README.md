 **前言** 
国内无法直接访问ChatGPT，只能通过科学上网的方式进行访问。
 **腾讯云-云函数** 
 通过腾讯云函数可以实现搭建一个代理服务。
  **操作步骤** 
  打开https://console.cloud.tencent.com/scf/list;选择新建
  
![lg949nmy.png](https://aiici.top/usr/uploads/2023/04/2529863456.png)
选择从头开始
![lg94auww.png](https://aiici.top/usr/uploads/2023/04/3955830533.png)
根据如图所示内容填写，选择web函数，地域建议国外，环境选择node16.13，然后选择本地zip包上传。包地址：https://github.com/aiici/chatgpt_proxy;现在zip包后上传。
![lg94ht0z.png](https://aiici.top/usr/uploads/2023/04/3931013270.png)
高级配置设置请求多并发
![lg94nlxj.png](https://aiici.top/usr/uploads/2023/04/567264616.png)
触发器选择默认就好，点完成创建即可！
![lg94ofw5.png](https://aiici.top/usr/uploads/2023/04/2774415565.png)
然后选择函数服务，触发管理，访问路径公网那个url就是你的代理地址。不需要后面的/release/
![lg94u2pq.png](https://aiici.top/usr/uploads/2023/04/243365646.png)
至此就完成搭建了，可以看到我们访问我们自己的代理地址和官网api.openai.com返回的数据是一样的！
![lg94w6cd.png](https://aiici.top/usr/uploads/2023/04/2677929642.png)
![lg94wpe1.png](https://aiici.top/usr/uploads/2023/04/348345601.png)

