# 企业后台人员管理系统
# 前端部分
## 主要基于vue 3.2.38框架实现，使用element-plus框架提供友好美化的互交操作。使⽤vuex管理全局数据状态，引入axios-mock-adapter模拟后端数据，通过axios拦截器实现请求全局异常处理。token保存在LocalStorage防止页面刷新登录数据丢失，基于后端返回的角色权限动态生成路由信息。

## 部署。前端服务部署在nginx docker容器，配置反向代理实现跨域请求；各端业务独立运行于含OpenJDK与MySQL 8的docker容器中，3个容器通过docker compose编排管理在同一桥接网络实现互交，实现环境隔离与弹性扩展。
