# loginWithGoogle
loginWithGoogle, 阿里云   API网关、函数计算  试用。

# 谷歌一键登录
如果你在浏览器里登录了谷歌的产品。那么就能使用谷歌一键登录，给其他的网站授权你的用户名、头像、邮箱。    


如果你的网络环境能正常访问谷歌，那么在[这个网站](https://feling.io)的右上角, 会出现登录按钮。    
这个登录按钮实际使用的就是这个项目里的代码，部署在了阿里云的API网关和函数计算上。    


# 试用评价
感觉函数计算目前的商业定位不在上层业务系统，而是图片处理之类的底层服务，内网访问vpc的功能还未上线。


访问量巨低的情况下，可能每次调用函数时，所有的实例都因为长时间没有被调用而被回收了。启动实例会增加5秒左右的响应时间，API网关也有这种现象。个人用户，自己定时调用接口，保证实例存活，基本能满足需求。企业用户，目测够呛。     



查看日志比较麻烦，官方推荐的方式是接入阿里云的日志服务，对于未使用过阿里云日志服务的人来说。。。太懒了。。不想看日志服务的文档了啊。。。     



按执行时间收费，对io型的业务系统来说，有种使不上劲的感觉。。请求个谷歌的http接口等了600ms，感觉啥都没干，600ms的钱就没了。。。     


发布代码的体验还是挺爽的，上面讲的缺点在我的使用场景里都不是什么大问题，所以整体还是好评的。
