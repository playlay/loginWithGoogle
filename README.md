# loginWithGoogle
loginWithGoogle, 阿里云   API网关、函数计算  试用。


感觉函数计算目前的商业定位不在上层业务系统，而是图片处理之类的底层服务，内网访问vpc的功能还未上线。  


访问量巨低的情况下，可能每次调用函数时，所有的实例都因为长时间没有被调用而被回收了。启动实例会增加5秒左右的响应时间。    


API网关也有这种现象