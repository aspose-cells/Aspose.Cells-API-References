---
title: "类 DataModelConnection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.ExternalConnections.DataModelConnection 类。指定数据模型连接"
type: docs
url: /zh/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

指定数据模型连接

```csharp
public class DataModelConnection : ExternalConnection
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | 指示连接是否可以在后台（异步）刷新。如果首选的使用方式是后台异步刷新，则为 true；如果首选的使用方式是前台同步刷新，则为 false。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | 获取此 [`ExternalConnection`](../externalconnection/) 对象的类型。 |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据 |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | 返回 [`OLEDBCommandType`](../oledbcommandtype/) 类型。 |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | 指定此连接的用户描述（继承自 [`ExternalConnection`](../externalconnection/)。） |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | 获取连接文件。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) 指定此连接的唯一标识符。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) 指定建立（或重新建立）连接时使用的身份验证方法。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | 指定建立（或重新建立）连接时使用的身份验证方法。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | 获取连接的 id。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | 指示关联的工作簿连接是否已被删除。如果连接已被删除，则为 true；否则为 false。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | 如果连接尚未首次刷新，则为 true；否则为 false。此状态可能在用户在查询完成返回之前保存文件时出现。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | 当电子表格应用程序应努力保持连接打开时为 true。为 false 时，应用程序应在检索信息后关闭连接。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | 指定连接的名称。每个连接必须具有唯一名称。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | 指定创建此连接的外部连接文件的完整路径。如果在尝试刷新数据期间连接失败，并且 reconnectionMethod=1，则电子表格应用程序将使用外部连接文件中的信息再次尝试，而不是使用嵌入工作簿的连接对象。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | 指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。如果为 false，则电子表格应用程序应遵循 reconnectionMethod 属性指示的程序。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | 获取 ODBC 或 Web 查询的 [`ConnectionParameterCollection`](../connectionparametercollection/)。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | 获取 Power Query 公式的定义。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) 指定当连接失败时电子表格应用程序应采取的操作。默认值为 ReConnectionMethodType.Required。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | 指定当连接失败时电子表格应用程序应采取的操作。默认值为 ReConnectionMethodType.Required。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | 指定连接自动刷新之间的分钟数。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | 如果在打开文件时应刷新此连接，则为 true；否则为 false。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | 如果要将通过连接获取的用于填充表格的外部数据与工作簿一起保存，则为 True；否则为 false。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | 如果要将密码作为连接字符串的一部分保存，则为 True；否则为 False。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | 指定在使用数据透视表基于服务器的页面字段时会被持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | 当外部数据源基于文件时使用。若对该数据源的连接失败，电子表格应用程序会尝试直接连接到此文件。可以使用 URI 或系统特定的文件路径表示。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | 获取或设置外部连接的数据源类型。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | 用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。（继承自 [`ExternalConnection`](../externalconnection/)。） |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**已过时。**) 获取或设置外部连接的数据源类型。（继承自 [`ExternalConnection`](../externalconnection/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();

            try
            {
                // 使用反射创建 DataModelConnection 类的实例
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // 设置必要属性
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // 将连接添加到工作簿的数据连接中
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // 显示连接信息
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // 保存工作簿
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


