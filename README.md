## 运维管理平台功能开发展示

<p align="center">
  <a href="https://golang.google.cn/">
    <img src="https://img.shields.io/badge/Django-3.4.12-green.svg" alt="django">
  </a>
  <a href="https://gin-gonic.com/">
    <img src="https://img.shields.io/badge/djangorestframework-3.12.4-green.svg" alt="djangorestframework">
  </a>
  <a href="https://redis.io/">
    <img src="https://img.shields.io/badge/redis-3.2.100-brightgreen.svg" alt="redis">
  </a>
  <a href="https://vuejs.org/">
    <img src="https://img.shields.io/badge/Vue-2.6.14-orange.svg" alt="vue">
  </a>
  <a href="https://antdv.com/docs/vue/introduce-cn/">
    <img src="https://img.shields.io/badge/ElementUI-2.13.12-green.svg" alt="elementui">
  </a>
</p>

> 本项目后端使用Django+DRF开发， 前端使用的是Vue2+ElementUI框架。

### 功能模块-系统管理
---
1. 菜单管理
实现菜单增删改查/菜单无感刷新/权限按钮
- 菜单总览
![image](https://user-images.githubusercontent.com/32893009/199173493-62650fa1-d25d-48c5-be27-01880cb8d2cc.png)

- 新增菜单
![image](https://user-images.githubusercontent.com/32893009/199173697-78410756-a311-469f-9edd-e35429aa3286.png)

2. 用户管理
实现LDAP用户对接/用户角色指定/用户激活/设置成超级管理员
- 用户总览
![image](https://user-images.githubusercontent.com/32893009/199173886-0689d14a-1ef9-4f99-aa96-4cd50fb7a509.png)

- 用户指定角色
![image](https://user-images.githubusercontent.com/32893009/199173960-b029e826-6d55-4e1f-b30e-624fff9592de.png)

3. 角色管理
实现角色的增删改查/角色列表查看与成员移除/前后端权限分配
- 角色总览
![image](https://user-images.githubusercontent.com/32893009/199174112-2655015e-59c2-4ace-aa20-e9640ef7f695.png)

- 角色成员查看与移除
![image](https://user-images.githubusercontent.com/32893009/199174136-f930bd6c-b297-4f17-881f-907b37418ab9.png)

- 后端权限分配
![image](https://user-images.githubusercontent.com/32893009/199174230-7591c07a-3d60-4518-953b-9c8c5cae9e65.png)

- 前端权限分配
![image](https://user-images.githubusercontent.com/32893009/199174351-530aae46-8afa-4c83-baff-194d3a84c06b.png)


### 功能模块-工作流管理
---
1. 工作流类型设计
实现工作流类型增删改查
- 总览
![image](https://user-images.githubusercontent.com/32893009/199174808-c5195eba-8d36-47e1-8b54-fafe3cd129da.png)

2. 工作流设计
- 实现工作流增删改查/工作流配置
![image](https://user-images.githubusercontent.com/32893009/199175074-5046394b-98ff-4e85-b250-9ad112170bcc.png)

- 配置工作流字段
![image](https://user-images.githubusercontent.com/32893009/199175199-0729e644-c8ba-4aa0-b05d-29fc0f4306d8.png)

- 配置工作流节点
![image](https://user-images.githubusercontent.com/32893009/199175287-a5c93035-5e87-4f1a-9c5a-ce7837c09e8f.png)

- 配置工作流步骤
![image](https://user-images.githubusercontent.com/32893009/199175320-9f3d0b8d-9d9e-4845-b8c1-4e7f1d8ec088.png)


### 功能模块-工单系统
---
已对接jenkins和gitlab，且实现了任务异步处理，消息通知等功能
1. 新建工单
![image](https://user-images.githubusercontent.com/32893009/199175492-f326a545-81a6-4c63-9e85-d9d35879d61b.png)

- 发布工单（关联gitlab和jenkins）
![image](https://user-images.githubusercontent.com/32893009/199175620-d3648b4c-1ab3-401a-9624-c186284b9459.png)
![image](https://user-images.githubusercontent.com/32893009/199175886-0bd1e62b-0111-46bc-9cfb-6cb373399542.png)

2. 我的工单
- 查询自己创建的工单
![image](https://user-images.githubusercontent.com/32893009/199175948-ccd31527-e92f-4d33-ad6d-32f506f0aee3.png)

3. 代办工单
- 查询待处理的工单
![image](https://user-images.githubusercontent.com/32893009/199176033-9ee2730a-c71c-4658-a0dc-9eb6516d9c40.png)

4. 全部工单
- 列出所有的工单
![image](https://user-images.githubusercontent.com/32893009/199176131-b4f70bf3-269a-49b6-8a8b-215560ff145d.png)


### 功能模块-cmdb
---
同步阿里云资产
1. 服务器管理
![image](https://user-images.githubusercontent.com/32893009/199176400-c938cbb1-d171-45d6-8013-c09e827fcc12.png)

2. 数据库管理
![image](https://user-images.githubusercontent.com/32893009/199176561-b8585c11-a656-441c-a55c-2c8e69c5f1c2.png)


### 功能模块-项目管理
---
同步gitlab中项目信息
![image](https://user-images.githubusercontent.com/32893009/199177025-1249a654-5701-4388-9af3-92e14f3efe0a.png)


### 功能模块-密码管理
---
- 以加密的方式记录公司所有账号密码，按权限组分配权限
![image](https://user-images.githubusercontent.com/32893009/199177648-219d8d34-2612-453f-a59a-5004d71173f5.png)

- 查询密码
![image](https://user-images.githubusercontent.com/32893009/199177694-f8235c03-01b2-4e64-b9f8-36fca3525aa8.png)



### 功能模块-K8S多集群管理
---
1. 多集群管理
![image](https://user-images.githubusercontent.com/32893009/199178126-c5a892e9-1b77-4398-9be6-df07d600f5ca.png)

2. 节点管理
![image](https://user-images.githubusercontent.com/32893009/199178207-b436637b-49b1-4ca2-88b4-f25b1c6f4247.png)


3. 工作负载
- pod终端/pod日志/文件上传下载/监控等功能
![image](https://user-images.githubusercontent.com/32893009/199178397-0e54647d-b05e-45f0-9d87-0da84a9c521a.png)

- 日志实时查询
![image](https://user-images.githubusercontent.com/32893009/199178614-a8445725-b553-46db-b416-a8f1fe7142b4.png)

- pod终端
![image](https://user-images.githubusercontent.com/32893009/199178733-59ded17b-671a-4f5c-a4e6-4638e4411a21.png)


4. 存储管理
![image](https://user-images.githubusercontent.com/32893009/199178801-38949410-a249-40cc-b9bd-d57e525e2865.png)


5. 网络管理
![image](https://user-images.githubusercontent.com/32893009/199178877-7cd1990f-59d5-441c-b1d7-de0e11d40594.png)
![image](https://user-images.githubusercontent.com/32893009/199179210-e332ede1-4fed-48b2-88bc-7b9e5c486756.png)


6. 事件管理
![image](https://user-images.githubusercontent.com/32893009/199179391-01445919-c7d3-466e-bcd9-6a6b04ae8fb3.png)

