---

copyright:
  years: 2016, 2018
lastupdated: "2018-02-23"

---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# 用户、应用程序和网关角色

角色是可用于授予或限制对特定操作的访问权的许可权集。使用角色可管理用户、应用程序和网关组的许可权。
{:shortdesc}

## 用户角色
{: #user_roles}

向 {{site.data.keyword.iot_full}} 添加、邀请或注册用户时，可分配用户角色。还可通过使用 {{site.data.keyword.iot_short_notm}} 仪表板随时分配或更改用户角色。有关向用户分配角色的更多信息，请参阅[管理用户角色](managing_user_roles.html)。

提供了以下标准用户角色：

用户角色|描述
------------- | -------------
管理员|授予对所有与用户相关的 API 的访问权的“超级用户”角色。管理员无法访问限于设备和应用程序的操作。

操作员|用于前端组织用户。授予对大多数组织操作、访问控制操作、第三方操作和风险管理操作的访问权。

开发者|授予对设备操作、日志操作、高速缓存操作、历史操作和第三方服务操作的不受限访问权。此角色提供对组织、访问控制和风险管理操作的限制访问权。
读者|缺省用户角色。授予对可用于所有用户的操作的受限访问权。



有关用户角色的更多信息，请参阅[用户角色](reference/roles_access.html)。

## 应用程序角色
{: #application_roles}
您可以分配应用程序角色以授予或拒绝应用程序对特定操作的访问权。所有应用程序角色都拒绝对以下操作的访问权：

- 所有风险管理操作
- 配置存储参数
- 配置认证服务提供者
- 创建、更新或删除电子邮件配置

提供了以下标准应用程序角色：

应用程序角色|描述
------------- | -------------
标准|缺省应用程序角色。授予对大多数应用程序操作（但不包括用户或角色操作）的访问权。
操作|授予对绝大多数操作的访问权，但拒绝对预订或发布操作的访问权。

可信后端|用于不需要系统操作员交互的应用程序。拒绝对设备管理、组织、角色或扩展操作的访问权。

数据处理器
|用于执行分析和数据处理的应用程序。数据处理器应用程序被授予对组织操作和用户操作的受限访问权。

可视化|用于负责生成数据可视化的应用程序。可视化应用程序对实时和存储数据操作及仪表板操作具有访问权。

设备|用于具有设备角色的应用程序；即，应用程序像设备一样提供发送到 {{site.data.keyword.iot_short_notm}} 的数据的源。设备应用程序仅被授予了对操作的受限访问权。


有关应用程序角色的操作访问权的更多信息，请参阅[应用程序角色](reference/app_roles_access.html)。

## 网关角色
{: #gateway_roles}
网关具有数量有限的角色，这些角色管理网关的定义以及向 {{site.data.keyword.iot_short_notm}} 注册设备的能力。

提供了以下标准网关角色：

网关角色|描述
------------- | -------------
标准|授予对操作的受限访问权。标准网关仅限于代表分配有资源组的网关中所包含的设备执行操作。
特权|缺省网关角色。用于可信网关，并允许特权网关向 {{site.data.keyword.iot_short_notm}} 添加设备。此角色授予了对用于添加、更新和管理设备及设备属性的相关操作的访问权，但不具有对其他操作的访问权。

有关网关角色的操作访问权的更多信息，请参阅[网关角色](reference/gateway_roles_access.html)。
