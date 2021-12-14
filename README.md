# LC_CPU
## CPU个数、内核数、线程数的区别
cpu个数是指物理上安装了几个cpu，一般的个人电脑是安装了1个cpu

cpu内核数是指物理上，一个cpu芯片上集成了几个内核单元，现代cpu都是多核的。

cpu线程数是指逻辑上处理单元，这个技术是Intel的超线程技术，它让操作系统识别到有多个处理单元。

如下图所示：插槽指cpu个数，内核数量是4个，线程数是4个。我的I5 4590 cpu不支持超线程技术。所以，一个内核就是一个线程。
![image](https://user-images.githubusercontent.com/26539681/145918698-b4224c2b-47e1-4c13-9068-03dc45dde564.png)
![image](https://user-images.githubusercontent.com/26539681/145918784-22f89ff2-a53d-4780-ad28-3d79d577d318.png)

CPU主频就是CPU运算时的工作频率，在单核时间它是决定CPU性能的重要指标，一般以MHz和GHz位单位，如Phenom II X4 965主频是3.4GHz。说到CPU主频，就不得不提外频和倍频的概念，它们的关系是：主频=外频×倍频。

虽然提高频率能有效提高CPU性能，但受限于制作工艺等物理因素，早在2004年，提高频率便遇到了瓶颈，于是Intel/AMD只能另辟途径来提升CPU性能，双核、多核CPU应运而生。

其实增加核心数目就是为了增加线程数，因为操作系统是通过线程来执行任务的，一般情况下它们是1:1对应关系，也就是说四核CPU一般拥有四个线程。但Intel引入超线程技术后，使核心数与线程数形成1:2的关系，如四核Core i7支持八线程(或叫作八个逻辑核心)，大幅提升了其多任务、多线程性能。

![image](https://user-images.githubusercontent.com/26539681/145919185-27aa3176-579f-41cf-9673-6978e6516570.png)
![image](https://user-images.githubusercontent.com/26539681/145919212-82ce1f39-3349-4fab-b735-53b6464b49da.png)
![image](https://user-images.githubusercontent.com/26539681/145919285-70f40f00-6f8f-4f43-b859-0c4b47fb2205.png)
