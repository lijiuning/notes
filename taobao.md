# 淘宝技术这十年

标签： 技术 读书笔记

---

# 0. 引言
> PV (page view) 页面访问量  
> UV (unique visitor) 用户访问量

```seq
Customer->DNS: www.taobao.com
DNS->Customer: the most fast server 192.168.1.1
Customer->Host:UV
Host->LVS:load balance (linux virtual server)
LVS->ReserveProxy:
ReserveProxy->RealServer:
RealServer->Customer: response HTML
Customer->CDN: static files request (content delivery network)
CDN->Customer: respond file
```

为了快速访问海量静态文件，开发了**分布式文件系统TFS**
为了及时迅速同步传输日志数据，开发了**TimeTunnel**
为了对海量交易、浏览数据进行分析，开发了**云梯** 基于Hadoop的超大规模数据系统
以及**ODPS**数据系统进行分析与挖掘


？mysql 的读写分离
？java mvc scruts
velocity ibatis hibernate EJB Spring JBOSS 

为了数据库分库（Oracle）能合并、排序、分页，开发了DBRoute
为了提升系统性能，开发了基于Berkeley DB的缓存系统，将静态 不太变化的数据放入


---

