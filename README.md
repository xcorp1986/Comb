# Comb
## 在为客户提供SaaS应用的时候你也许会有如下需求
1. 为不同客户分配不同的子域名。<br> 例如:<br>客户A使用 https://a.domain.com , <br>客户B使用 https://b.domain.com , <br>... ,<br> 客户N使用 https://n.domain.com
2. 服务端为客户A和客户B（客户N）提供完全相互独立，物理隔离的应用
3. 基于上面一点，特殊定制某个客户的需求，并不影响其他客户
4. 迭代升级可以灰度升级
5. 升级和回退版本都直观安全
6. 监控每个客户系统资源状况
7. 新增或者修改客户二级域名代理时，不会中断对外服务（不重启Nginx）

### 架构拓扑图如下所示
![alt 架构和拓扑图](https://github.com/fjb040911/Comb/blob/master/docImgs/jg.png)
