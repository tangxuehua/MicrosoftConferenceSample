MicrosoftConferenceSample
=========================

The sample from microsoft cqrs journey sample code.

运行步骤：
1. 编译源代码；
2. 新建一个conference数据库，然后执行scripts目录下的那两个SQL脚本，创建数据库表；
3. 总共有三个宿主工程分别是：
   1）Conference.Web.Admin， 用于会议以及每个会议的位置信息的后台管理；
   2）Conference.Web.Public，用于会议以及每个会议的位置信息的前台展示，同时提供预订会议位置的功能；
   3）WorkerRoleCommandProcessor，该项目是一个控制台服务，用于负责监听上面这两个站点所产生的消息，然后调用相关的消息消费者进行处理；

以上三个宿主工程都运行起来，就能进行操作了。