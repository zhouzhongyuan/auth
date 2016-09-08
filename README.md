## 登录的简单实现

### 理解

![session原理](assets/session原理.jpg)

### 时间

### 参考

[The definitive guide to form-based website authentication](http://stackoverflow.com/questions/549/the-definitive-guide-to-form-based-website-authentication)

#### 2016-09-06
- store用来存储session状态(memory.js)
- res.end: 相当于扩展了res.end的功能
- 画流程图是个研究别人代码的好方法
- **把别人的代码改成自己的代码才是研究别人代码的好方法**


### TODO

登录过程的流程图

### 问题
1. 问:createSession的作用是什么?

   答:每个请求都要新建一个会话。
   
2. 问:express中间件返回一个function的作用是什么?

   答:具体不知道啊,类似于 `next()`
3. 问:req.session.user为什么可以用来作为判断是否登录的依据呢?

   答:因为成功登录的时候,会把user信息存到sessions中;登录失败的session不会保存user信息到sessions中去