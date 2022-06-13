---
title: WebQueryConnection
second_title: Aspose.Cells for .NET API 参考
description: 指定 Web 查询源的属性 Web 查询将从 HTML 表 中检索数据并且还可以提供 HTTPGet参数以供 Web 服务器在通过 生成 HTML 时处理包括参数和参数元素
type: docs
weight: 3350
url: /zh/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

指定 Web 查询源的属性。 Web 查询将从 HTML 表 中检索数据，并且还可以提供 HTTP“Get”参数以供 Web 服务器在通过 生成 HTML 时处理，包括参数和参数元素。

```csharp
public class WebQueryConnection : ExternalConnection
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | 表示是否可以在后台（异步）刷新连接。 如果连接的首选用法是在后台异步刷新，则为 true； 如果连接的首选用法是在前台同步刷新，则为 false。 |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | 指定此连接的用户描述 |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | 指定此连接的唯一标识符。 |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | 指定建立（或重新建立）连接时要使用的身份验证方法。 |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | 显示网络查询数据的面向用户的网页的 URL。在 sourceData="true" 和 url 已被重定向以引用 XML 文件的情况下，此 URL 将保留为 。 然后可以在 UI 中显示面向用户的页面，并且可以在后台检索 XML 数据 。 |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | 在将 Web 查询数据引入 工作表时如何处理来自 HTML 源的格式设置。当 sourceData 为 True 时相关。 |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | 获取连接的ID。 |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | 指示连续分隔符是否应仅视为一个分隔符的标志。 |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | 指示关联的工作簿连接是否已被删除。如果 连接已被删除，则为 true；否则为假。 |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | 指示 Web 查询是否应仅适用于 HTML 表的标志。 |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | 如果连接没有第一次刷新，则为真；否则为假。 当用户在查询完成返回之前保存文件时，可能会发生这种状态。 |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | 指示网页中 HTML PRE 标记中包含的数据是否为 在将页面导入查询表时解析为列的标志。 |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | 标志，指示是否解析 PRE 块内的所有表，其宽度设置 与第一行相同。 |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | 指示日期是否应作为文本而不是日期导入工作表中的单元格的标志。 |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | 此标志的存在是为了向后兼容旧的现有电子表格文件，如果此 Web 查询在较新的电子表格应用程序中刷新，则将 设置为 true大于或等于 到 Microsoft Excel 2000。 这是一个可以忽略的可选属性。 |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | 此标志的存在是为了向后兼容旧的现有电子表格文件，如果此 Web 查询是在 Microsoft Excel 97 中创建的，则将 设置为 true。 这是一个可以忽略的可选属性。 |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | 如果 Web 查询源是 XML（相对于 HTML），则为 true，否则为 false。 |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | 指示应导入 XML 源数据而不是 HTML 表本身的标志。 |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | 当电子表格应用程序应努力保持连接 打开时为真。当为 false 时，应用程序应在检索到 信息后关闭连接。 |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | 指定连接的名称。每个连接都必须有一个唯一的名称。 |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | 指定创建此连接的外部连接文件的完整路径 。如果在尝试刷新数据期间连接失败，并且 reconnectionMethod=1, 则电子表格应用程序将使用来自外部连接文件 的信息而不是嵌入的连接对象再次尝试工作簿内。 |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | 指示电子表格应用程序是否应始终且仅使用 odcFile 属性:::47 指示的外部连接文件中的 连接信息:::刷新连接时。如果为 false，则电子表格应用程序 应遵循 reconnectionMethod 属性 |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | 获取[`ConnectionParameterCollection`](../connectionparametercollection)用于 ODBC 或 Web 查询。 |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | 返回或设置用于将数据输入到 Web 服务器的 post 方法的字符串 从 Web 查询返回数据。 |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | 获取幂查询公式的定义。 |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | 指定电子表格应用程序在连接失败时应该做什么。 默认值为 ReConnectionMethodType.Required。 |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | 指定连接自动刷新之间的分钟数。 |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | 如果在打开文件时应该刷新此连接，则为真；否则为假。 |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | 如果通过连接获取的用于填充表的外部数据要与工作簿一起保存 则为真；否则为假。 |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | 如果密码要保存为连接字符串的一部分，则为真；否则为假。 |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | 当外部数据源基于文件时使用。当与此类数据 源的连接失败时，电子表格应用程序会尝试直接连接到该文件。可能是 以 URI 或系统特定的文件路径表示法表示。 |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | 单点登录 (SSO) 标识符，用于在中间 电子表格机器学习服务器和外部数据源之间进行身份验证。 |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | 获取或设置外部连接数据源类型。 |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | 用于刷新外部数据的 URL。 |

### 也可以看看

* class [ExternalConnection](../externalconnection)
* 命名空间 [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
