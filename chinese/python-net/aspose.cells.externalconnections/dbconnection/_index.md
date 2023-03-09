---
title: DBConnection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
## DBConnection类
指定与 ODBC 或 OLE DB 外部数据连接关联的所有属性。



**继承：** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)



DBConnection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [id](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/id) |获取连接的 ID。|
| [power_query_formula](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) |获取幂查询公式的定义。|
| [type](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/type) |获取或设置外部连接数据源类型。|
| [source_file](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/source_file) |当外部数据源是基于文件的时使用。<br/> source 失败，电子表格应用程序尝试直接连接到该文件。<br/>以 URI 或系统特定的文件路径表示法表示。|
| [sso_id](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/sso_id) |用于中间体之间身份验证的单点登录 (SSO) 标识符<br/>spreadsheetML 服务器和外部数据源。|
| [save_password](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/save_password) |如果要将密码保存为连接字符串的一部分，则为 True；否则为 False。|
| [save_data](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/save_data) |如果要保存通过连接获取的用于填充表的外部数据，则为真<br/>与工作簿一起；否则，错误。|
| [refresh_on_load](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) |如果在打开文件时应刷新此连接，则为真；否则为真。|
| [reconnection_method_type](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) |指定当连接失败时电子表格应用程序应该做什么。<br/>默认值为 ReConnectionMethodType.Required。|
| [reconnection_method](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) |指定当连接失败时电子表格应用程序应该做什么。<br/>默认值为 ReConnectionMethodType.Required。|
| [only_use_connection_file](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) |指示电子表格应用程序是否应始终且仅使用<br/>odcFile 属性指示的外部连接文件中的连接信息<br/>当连接刷新时。如果为 false，则电子表格应用程序<br/>应遵循 reconnectionMethod 属性指示的过程|
| [odc_file](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/odc_file) |指定此连接来自的外部连接文件的完整路径<br/>如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，<br/>然后电子表格应用程序将使用来自外部连接文件的信息重试<br/>而不是工作簿中嵌入的连接对象。|
| [is_new](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/is_new) |如果连接不是第一次刷新，则为 True；否则为 false。<br/>当用户在查询完成返回之前保存文件时，就会发生这种状态。|
| [name](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/name) |指定连接的名称。|
| [keep_alive](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) |当电子表格应用程序应努力保持连接时为真<br/>打开。如果为 false，应用程序应在检索到<br/>信息。|
| [refresh_internal](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) |指定连接自动刷新之间的分钟数。|
| [connection_id](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/connection_id) |指定此连接的唯一标识符。|
| [connection_description](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/connection_description) |指定此连接的用户描述|
| [is_deleted](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |指示关联的工作簿连接是否已被删除。如果<br/>否则，假的。|
| [credentials_method_type](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) |指定建立（或重新建立）连接时要使用的身份验证方法。|
| [credentials](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/credentials) |指定建立（或重新建立）连接时要使用的身份验证方法。|
| [background_refresh](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) |指示是否可以在后台（异步）刷新连接。<br/>如果连接的首选用法是在后台异步刷新，则为真；<br/>如果连接的首选用法是在前台同步刷新，则为 false。|
| [parameters](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/parameters) |为 ODBC 或 Web 查询获取 [ConnectionParameterCollection](/cells/zh/python-net/aspose.cells.externalconnections/connectionparametercollection)。|
| [connection_info](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/connection_info) |连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。|
| [command_type](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/command_type) |指定 OLE DB 命令类型。<br/>1.查询指定一个cube名称<br/>2.Query指定一条SQL语句<br/>3.查询指定表名<br/>4. Query指定已经给出了默认信息，由provider如何解读。<br/>5. 查询针对基于 Web 的列表数据提供程序。|
| [command](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/command) |包含要传递给数据提供者 API 的数据库命令的字符串<br/>与外部源交互以检索数据|
| [sever_command](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |指定第二个命令文本字符串，当数据透视表基于服务器时持久化<br/>页字段正在使用中。<br/>对于 ODBC 连接，serverCommand 通常是比命令更广泛的查询（没有<br/>WHERE 子句存在于前者中）。<br/>可以填充参数 UI 并可以构造参数化查询|



### 也可以看看
* 模块 [aspose.cells.externalconnections](..)
* 类 [ConnectionParameterCollection](/cells/zh/python-net/aspose.cells.externalconnections/connectionparametercollection)
* 类 [DBConnection](/cells/zh/python-net/aspose.cells.externalconnections/dbconnection)
* 类 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)
