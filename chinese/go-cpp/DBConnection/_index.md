---
title: "DBConnection 类"
linktitle: "DBConnection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DBConnection 类。封装在 Go 中表示 dbconnection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/dbconnection/
---

## DBConnection class

指定与 ODBC 或 OLE DB 外部数据连接关联的所有属性。

```go

type DBConnection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDBConnection](./newdbconnection/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetClassType](./getclasstype/) | 获取此 ExternalConnection 对象的类型。 |
| [GetConnectionString](./getconnectionstring/) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [SetConnectionString](./setconnectionstring/) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [GetPowerQueryFormula](./getpowerqueryformula/) | 获取 Power Query 公式的定义。 |
| [GetCommandType](./getcommandtype/) | 指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名 4. 查询指定已提供默认信息，由提供程序自行解释 5. 查询针对基于 Web 的 List Data Provider。 |
| [SetCommandType](./setcommandtype/) | 指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名 4. 查询指定已提供默认信息，由提供程序自行解释 5. 查询针对基于 Web 的 List Data Provider。 |
| [GetCommand](./getcommand/) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [SetCommand](./setcommand/) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [GetSecondCommand](./getsecondcommand/) | 指定在使用 PivotTable 服务器端页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。 |
| [SetSecondCommand](./setsecondcommand/) | 指定在使用 PivotTable 服务器端页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。 |
| [GetId](./getid/) | 获取连接的 id。 |
| [GetSourceType](./getsourcetype/) | 获取或设置外部连接的 DataSource 类型。 |
| [SetSourceType](./setsourcetype/) | 获取或设置外部连接的 DataSource 类型。 |
| [GetSSOId](./getssoid/) | 用于在 intermediate spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。 |
| [SetSSOId](./setssoid/) | 用于在 intermediate spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。 |
| [GetSavePassword](./getsavepassword/) | 如果密码应作为连接字符串的一部分保存，则为 True；否则为 False。 |
| [SetSavePassword](./setsavepassword/) | 如果密码应作为连接字符串的一部分保存，则为 True；否则为 False。 |
| [GetSaveData](./getsavedata/) | 如果通过连接获取的用于填充表格的外部数据应随工作簿一起保存，则为 True；否则为 false。 |
| [SetSaveData](./setsavedata/) | 如果通过连接获取的用于填充表格的外部数据应随工作簿一起保存，则为 True；否则为 false。 |
| [GetRefreshOnLoad](./getrefreshonload/) | 如果在打开文件时应刷新此连接，则为 True；否则为 false。 |
| [SetRefreshOnLoad](./setrefreshonload/) | 如果在打开文件时应刷新此连接，则为 True；否则为 false。 |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | 指定电子表格应用在连接失败时应执行的操作。默认值为 ReConnectionMethodType.Required。 |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | 指定电子表格应用在连接失败时应执行的操作。默认值为 ReConnectionMethodType.Required。 |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | 指示在刷新连接时，电子表格应用是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。如果为 false，则电子表格应用应遵循 reconnectionMethod 属性指示的过程。 |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | 指示在刷新连接时，电子表格应用是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。如果为 false，则电子表格应用应遵循 reconnectionMethod 属性指示的过程。 |
| [GetOdcFile](./getodcfile/) | 指定创建此连接的外部连接文件的完整路径。如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，电子表格应用将使用外部连接文件中的信息重新尝试，而不是使用嵌入工作簿的连接对象。 |
| [SetOdcFile](./setodcfile/) | 指定创建此连接的外部连接文件的完整路径。如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，电子表格应用将使用外部连接文件中的信息重新尝试，而不是使用嵌入工作簿的连接对象。 |
| [GetSourceFile](./getsourcefile/) | 当外部数据源基于文件时使用。如果此类数据源的连接失败，电子表格应用会尝试直接连接该文件。可以使用 URI 或系统特定的文件路径表示法。 |
| [SetSourceFile](./setsourcefile/) | 当外部数据源基于文件时使用。如果此类数据源的连接失败，电子表格应用会尝试直接连接该文件。可以使用 URI 或系统特定的文件路径表示法。 |
| [IsNew](./isnew/) | 如果连接尚未首次刷新，则为 True；否则为 false。此状态可能在用户在查询返回完成前保存文件时出现。 |
| [SetIsNew](./setisnew/) | 如果连接尚未首次刷新，则为 True；否则为 false。此状态可能在用户在查询返回完成前保存文件时出现。 |
| [GetName](./getname/) | 指定连接的名称。每个连接必须拥有唯一的名称。 |
| [SetName](./setname/) | 指定连接的名称。每个连接必须拥有唯一的名称。 |
| [GetKeepAlive](./getkeepalive/) | 当电子表格应用应努力保持连接打开时为 True；为 false 时，应用应在检索信息后关闭连接。 |
| [SetKeepAlive](./setkeepalive/) | 当电子表格应用应努力保持连接打开时为 True；为 false 时，应用应在检索信息后关闭连接。 |
| [GetRefreshInternal](./getrefreshinternal/) | 指定连接自动刷新之间的间隔分钟数。 |
| [SetRefreshInternal](./setrefreshinternal/) | 指定连接自动刷新之间的间隔分钟数。 |
| [GetConnectionDescription](./getconnectiondescription/) | 指定此连接的用户描述 |
| [SetConnectionDescription](./setconnectiondescription/) | 指定此连接的用户描述 |
| [IsDeleted](./isdeleted/) | 指示关联的工作簿连接是否已被删除。如果连接已被删除则为 true；否则为 false。 |
| [SetIsDeleted](./setisdeleted/) | 指示关联的工作簿连接是否已被删除。如果连接已被删除则为 true；否则为 false。 |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | 指定建立（或重新建立）连接时使用的身份验证方法。 |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | 指定建立（或重新建立）连接时使用的身份验证方法。 |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | 指示连接是否可以在后台（异步）刷新。如果首选的使用方式是在后台异步刷新，则为 true；如果首选的使用方式是在前台同步刷新，则为 false。 |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | 指示连接是否可以在后台（异步）刷新。如果首选的使用方式是在后台异步刷新，则为 true；如果首选的使用方式是在前台同步刷新，则为 false。 |
| [GetParameters](./getparameters/) | 获取 ODBC 或 Web 查询的 ConnectionParameterCollection。 |
| [GetConnectionFile](./getconnectionfile/) | 获取连接文件。 |
