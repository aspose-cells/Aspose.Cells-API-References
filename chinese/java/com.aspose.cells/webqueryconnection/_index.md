---
title: "WebQueryConnection"
second_title: "Aspose.Cells for Java API 参考"
description: "指定 web 查询源的属性。"
type: docs
url: /zh/java/com.aspose.cells/webqueryconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class WebQueryConnection extends ExternalConnection
```

指定 Web 查询源的属性。Web 查询将从 HTML 表格检索数据，并且还可以提供 HTTP \"Get\" 参数，由 Web 服务器在生成 HTML 时处理这些参数和参数元素。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | 指示连接是否可以在后台（异步）刷新。 |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | 获取此 [ExternalConnection](../../com.aspose.cells/externalconnection) 对象的类型。 |
| [getCommand()](#getCommand--) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [getCommandType()](#getCommandType--) | 指定 OLE DB 命令类型。1。 |
| [getConnectionDescription()](#getConnectionDescription--) | 指定此连接的用户描述 |
| [getConnectionFile()](#getConnectionFile--) | 获取连接文件。 |
| [getConnectionId()](#getConnectionId--) | 指定此连接的唯一标识符。 |
| [getConnectionString()](#getConnectionString--) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [getCredentials()](#getCredentials--) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [getEditPage()](#getEditPage--) | 显示 Web 查询数据的面向用户的网页的 URL。 |
| [getEditWebPage()](#getEditWebPage--) | 显示 Web 查询数据的面向用户的网页的 URL。 |
| [getHtmlFormat()](#getHtmlFormat--) | 将 Web 查询数据导入工作表时，如何处理来自 HTML 源的格式。 |
| [getId()](#getId--) | 获取连接的 ID。 |
| [getKeepAlive()](#getKeepAlive--) | 当电子表格应用程序应努力保持连接打开时为 true。 |
| [getName()](#getName--) | 指定连接的名称。 |
| [getOdcFile()](#getOdcFile--) | 指定创建此连接的外部连接文件的完整路径。 |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | 指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。 |
| [getParameters()](#getParameters--) | 获取用于 ODBC 或 Web 查询的 [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)。 |
| [getPost()](#getPost--) | 返回或设置用于通过 POST 方法向 Web 服务器输入数据以返回 Web 查询数据的字符串。 |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | 获取 Power Query 公式的定义。 |
| [getReconnectionMethod()](#getReconnectionMethod--) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [getRefreshInternal()](#getRefreshInternal--) | 指定连接自动刷新之间的分钟数。 |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | 如果在打开文件时应刷新此连接则为 true；否则为 false。 |
| [getSSOId()](#getSSOId--) | 用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。 |
| [getSaveData()](#getSaveData--) | 如果通过连接获取的用于填充表格的外部数据要随工作簿一起保存，则为 true；否则为 false。 |
| [getSavePassword()](#getSavePassword--) | 如果密码要作为连接字符串的一部分保存，则为 true；否则为 false。 |
| [getSecondCommand()](#getSecondCommand--) | 指定在使用基于服务器的透视表页面字段时持久化的第二个命令文本字符串。 |
| [getSourceFile()](#getSourceFile--) | 当外部数据源基于文件时使用。 |
| [getSourceType()](#getSourceType--) | 获取外部连接的数据源类型。 |
| [getType()](#getType--) | 获取外部连接的数据源类型。 |
| [getUrl()](#getUrl--) | 用于刷新外部数据的 URL。 |
| [hashCode()](#hashCode--) |  |
| [isConsecutive()](#isConsecutive--) | 指示是否将连续的分隔符视为单个分隔符的标志。 |
| [isDeleted()](#isDeleted--) | 指示关联的工作簿连接是否已被删除。 |
| [isHtmlTables()](#isHtmlTables--) | 指示 Web 查询是否仅在 HTML 表格上工作的标志。 |
| [isNew()](#isNew--) | 如果连接尚未首次刷新则为 true；否则为 false。 |
| [isParsePre()](#isParsePre--) | 指示在将网页导入查询表时，网页中 HTML PRE 标签内的数据是否被解析为列的标志。 |
| [isSameSettings()](#isSameSettings--) | 指示是否使用与第一行相同的宽度设置解析 PRE 块内所有表格的标志。 |
| [isTextDates()](#isTextDates--) | 指示是否将日期作为文本而非日期导入工作表单元格的标志。 |
| [isXl2000()](#isXl2000--) | 此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询在 Microsoft Excel 2000 或更高版本的电子表格应用程序中刷新，则设置为 true。 |
| [isXl97()](#isXl97--) | 此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询是在 Microsoft Excel 97 中创建的，则设置为 true。 |
| [isXml()](#isXml--) | 如果网络查询源是 XML（而非 HTML），则为 true，否则为 false。 |
| [isXmlSourceData()](#isXmlSourceData--) | 指示应导入 XML 源数据而不是 HTML 表本身的标志。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | 指示连接是否可以在后台（异步）刷新。 |
| [setCommand(String value)](#setCommand-java.lang.String-) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [setCommandType(int value)](#setCommandType-int-) | 指定 OLE DB 命令类型。1。 |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | 指定此连接的用户描述 |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [setConsecutive(boolean value)](#setConsecutive-boolean-) | 指示是否将连续的分隔符视为单个分隔符的标志。 |
| [setCredentials(int value)](#setCredentials-int-) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [setDeleted(boolean value)](#setDeleted-boolean-) | 指示关联的工作簿连接是否已被删除。 |
| [setEditPage(String value)](#setEditPage-java.lang.String-) | 显示 Web 查询数据的面向用户的网页的 URL。 |
| [setEditWebPage(String value)](#setEditWebPage-java.lang.String-) | 显示 Web 查询数据的面向用户的网页的 URL。 |
| [setHtmlFormat(int value)](#setHtmlFormat-int-) | 将 Web 查询数据导入工作表时，如何处理来自 HTML 源的格式。 |
| [setHtmlTables(boolean value)](#setHtmlTables-boolean-) | 指示 Web 查询是否仅在 HTML 表格上工作的标志。 |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | 当电子表格应用程序应努力保持连接打开时为 true。 |
| [setName(String value)](#setName-java.lang.String-) | 指定连接的名称。 |
| [setNew(boolean value)](#setNew-boolean-) | 如果连接尚未首次刷新则为 true；否则为 false。 |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | 指定创建此连接的外部连接文件的完整路径。 |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | 指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。 |
| [setParsePre(boolean value)](#setParsePre-boolean-) | 指示在将网页导入查询表时，网页中 HTML PRE 标签内的数据是否被解析为列的标志。 |
| [setPost(String value)](#setPost-java.lang.String-) | 返回或设置用于通过 POST 方法向 Web 服务器输入数据以返回 Web 查询数据的字符串。 |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | 指定连接自动刷新之间的分钟数。 |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | 如果在打开文件时应刷新此连接则为 true；否则为 false。 |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | 用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。 |
| [setSameSettings(boolean value)](#setSameSettings-boolean-) | 指示是否使用与第一行相同的宽度设置解析 PRE 块内所有表格的标志。 |
| [setSaveData(boolean value)](#setSaveData-boolean-) | 如果通过连接获取的用于填充表格的外部数据要随工作簿一起保存，则为 true；否则为 false。 |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | 如果密码要作为连接字符串的一部分保存，则为 true；否则为 false。 |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | 指定在使用基于服务器的透视表页面字段时持久化的第二个命令文本字符串。 |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | 当外部数据源基于文件时使用。 |
| [setSourceType(int value)](#setSourceType-int-) | 设置外部连接的数据源类型。 |
| [setTextDates(boolean value)](#setTextDates-boolean-) | 指示是否将日期作为文本而非日期导入工作表单元格的标志。 |
| [setType(int value)](#setType-int-) | 设置外部连接的数据源类型。 |
| [setUrl(String value)](#setUrl-java.lang.String-) | 用于刷新外部数据的 URL。 |
| [setXl2000(boolean value)](#setXl2000-boolean-) | 此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询在 Microsoft Excel 2000 或更高版本的电子表格应用程序中刷新，则设置为 true。 |
| [setXl97(boolean value)](#setXl97-boolean-) | 此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询是在 Microsoft Excel 97 中创建的，则设置为 true。 |
| [setXml(boolean value)](#setXml-boolean-) | 如果网络查询源是 XML（而非 HTML），则为 true，否则为 false。 |
| [setXmlSourceData(boolean value)](#setXmlSourceData-boolean-) | 指示应导入 XML 源数据而不是 HTML 表本身的标志。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


指示连接是否可以在后台（异步）刷新。如果首选的使用方式是在后台异步刷新则为 true；如果首选的使用方式是在前台同步刷新则为 false。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClassType() {#getClassType--}
```
public int getClassType()
```


获取此 [ExternalConnection](../../com.aspose.cells/externalconnection) 对象的类型。

参见 [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype)。

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名称 4. 查询指定已提供默认信息，由提供程序决定如何解释。5. 查询针对基于 Web 的列表数据提供程序。

参见 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype)。

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


指定此连接的用户描述

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


获取连接文件。

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


指定此连接的唯一标识符。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.Id 属性。此属性将在自 2024 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


指定在建立（或重新建立）连接时使用的身份验证方法。

参见 [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.CredentialsMethodType 属性。此属性将在自 2017 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


指定在建立（或重新建立）连接时使用的身份验证方法。

参见 [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype)。

**Returns:**
int
### getEditPage() {#getEditPage--}
```
public String getEditPage()
```


显示网络查询数据的面向用户的网页的 URL。如果 sourceData=\"true\" 且 url 已被重定向以引用 XML 文件，则此 URL 会被保留。这样即可在 UI 中显示面向用户的页面，并在后台检索 XML 数据。

**Remarks**

注意：此属性现已废弃。请改用 WebQueryConnection.EditWebPage 属性。自 2017 年 10 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getEditWebPage() {#getEditWebPage--}
```
public String getEditWebPage()
```


显示网络查询数据的面向用户的网页的 URL。如果 sourceData=\"true\" 且 url 已被重定向以引用 XML 文件，则此 URL 会被保留。这样即可在 UI 中显示面向用户的页面，并在后台检索 XML 数据。

**Returns:**
java.lang.String
### getHtmlFormat() {#getHtmlFormat--}
```
public int getHtmlFormat()
```


在将网络查询数据导入工作表时，如何处理来自 HTML 源的格式。当 sourceData 为 True 时相关。

参见 [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype)。

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


获取连接的 ID。

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


当电子表格应用程序应努力保持连接打开时为 True。为 False 时，应用程序应在检索信息后关闭连接。

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


指定连接的名称。每个连接必须具有唯一名称。

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


指定创建此连接的外部连接文件的完整路径。如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，则电子表格应用程序将尝试使用外部连接文件中的信息再次连接，而不是使用工作簿中嵌入的连接对象。

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。若为 False，则电子表格应用程序应遵循 reconnectionMethod 属性指示的过程。

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


获取用于 ODBC 或 Web 查询的 [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)。

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPost() {#getPost--}
```
public String getPost()
```


返回或设置用于通过 POST 方法向 Web 服务器输入数据以返回 Web 查询数据的字符串。

**Returns:**
java.lang.String
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


获取 Power Query 公式的定义。

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


指定当连接失败时电子表格应用程序应执行的操作。默认值为 ReConnectionMethodType.Required。

参见 [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.ReconnectionMethodType 属性。此属性将在自 2017 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


指定当连接失败时电子表格应用程序应执行的操作。默认值为 ReConnectionMethodType.Required。

参见 [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype)。

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


指定连接自动刷新之间的分钟数。

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


如果在打开文件时应刷新此连接则为 true；否则为 false。

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


如果通过连接获取的用于填充表格的外部数据要随工作簿一起保存，则为 true；否则为 false。

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


如果密码要作为连接字符串的一部分保存，则为 true；否则为 false。

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


指定在使用数据透视表基于服务器的页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


当外部数据源基于文件时使用。如果此类数据源的连接失败，电子表格应用程序会尝试直接连接到该文件。可以使用 URI 或系统特定的文件路径表示法。

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


获取外部连接的数据源类型。

参见 [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype)。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取外部连接的数据源类型。

参见 [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.SourceType 属性。此属性将在自 2024 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getUrl() {#getUrl--}
```
public String getUrl()
```


用于刷新外部数据的 URL。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isConsecutive() {#isConsecutive--}
```
public boolean isConsecutive()
```


指示是否将连续的分隔符视为单个分隔符的标志。

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


指示关联的工作簿连接是否已被删除。若已删除则为 true；否则为 false。

**Returns:**
boolean
### isHtmlTables() {#isHtmlTables--}
```
public boolean isHtmlTables()
```


指示 Web 查询是否仅在 HTML 表格上工作的标志。

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


如果连接尚未首次刷新则为 True；否则为 false。当用户在查询完成返回前保存文件时可能出现此状态。

**Returns:**
boolean
### isParsePre() {#isParsePre--}
```
public boolean isParsePre()
```


指示在将网页导入查询表时，网页中 HTML PRE 标签内的数据是否被解析为列的标志。

**Returns:**
boolean
### isSameSettings() {#isSameSettings--}
```
public boolean isSameSettings()
```


指示是否使用与第一行相同的宽度设置解析 PRE 块内所有表格的标志。

**Returns:**
boolean
### isTextDates() {#isTextDates--}
```
public boolean isTextDates()
```


指示是否将日期作为文本而非日期导入工作表单元格的标志。

**Returns:**
boolean
### isXl2000() {#isXl2000--}
```
public boolean isXl2000()
```


此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询在 Microsoft Excel 2000 或更高版本的电子表格应用程序中刷新，则设置为 true。此为可选属性，可忽略。

**Returns:**
boolean
### isXl97() {#isXl97--}
```
public boolean isXl97()
```


此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询是在 Microsoft Excel 97 中创建的，则设置为 true。此为可选属性，可忽略。

**Returns:**
boolean
### isXml() {#isXml--}
```
public boolean isXml()
```


如果网络查询源是 XML（而非 HTML），则为 true，否则为 false。

**Returns:**
boolean
### isXmlSourceData() {#isXmlSourceData--}
```
public boolean isXmlSourceData()
```


指示应导入 XML 源数据而不是 HTML 表本身的标志。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundRefresh(boolean value) {#setBackgroundRefresh-boolean-}
```
public void setBackgroundRefresh(boolean value)
```


指示连接是否可以在后台（异步）刷新。如果首选的使用方式是在后台异步刷新则为 true；如果首选的使用方式是在前台同步刷新则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名称 4. 查询指定已提供默认信息，由提供程序决定如何解释。5. 查询针对基于 Web 的列表数据提供程序。

参见 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


指定此连接的用户描述

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setConsecutive(boolean value) {#setConsecutive-boolean-}
```
public void setConsecutive(boolean value)
```


指示是否将连续的分隔符视为单个分隔符的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


指定在建立（或重新建立）连接时使用的身份验证方法。

参见 [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.CredentialsMethodType 属性。此属性将在自 2017 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


指定在建立（或重新建立）连接时使用的身份验证方法。

参见 [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


指示关联的工作簿连接是否已被删除。若已删除则为 true；否则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEditPage(String value) {#setEditPage-java.lang.String-}
```
public void setEditPage(String value)
```


显示网络查询数据的面向用户的网页的 URL。如果 sourceData=\"true\" 且 url 已被重定向以引用 XML 文件，则此 URL 会被保留。这样即可在 UI 中显示面向用户的页面，并在后台检索 XML 数据。

**Remarks**

注意：此属性现已废弃。请改用 WebQueryConnection.EditWebPage 属性。自 2017 年 10 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setEditWebPage(String value) {#setEditWebPage-java.lang.String-}
```
public void setEditWebPage(String value)
```


显示网络查询数据的面向用户的网页的 URL。如果 sourceData=\"true\" 且 url 已被重定向以引用 XML 文件，则此 URL 会被保留。这样即可在 UI 中显示面向用户的页面，并在后台检索 XML 数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHtmlFormat(int value) {#setHtmlFormat-int-}
```
public void setHtmlFormat(int value)
```


在将网络查询数据导入工作表时，如何处理来自 HTML 源的格式。当 sourceData 为 True 时相关。

参见 [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHtmlTables(boolean value) {#setHtmlTables-boolean-}
```
public void setHtmlTables(boolean value)
```


指示 Web 查询是否仅在 HTML 表格上工作的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


当电子表格应用程序应努力保持连接打开时为 True。为 False 时，应用程序应在检索信息后关闭连接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


指定连接的名称。每个连接必须具有唯一名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


如果连接尚未首次刷新则为 True；否则为 false。当用户在查询完成返回前保存文件时可能出现此状态。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


指定创建此连接的外部连接文件的完整路径。如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，则电子表格应用程序将尝试使用外部连接文件中的信息再次连接，而不是使用工作簿中嵌入的连接对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。若为 False，则电子表格应用程序应遵循 reconnectionMethod 属性指示的过程。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setParsePre(boolean value) {#setParsePre-boolean-}
```
public void setParsePre(boolean value)
```


指示在将网页导入查询表时，网页中 HTML PRE 标签内的数据是否被解析为列的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPost(String value) {#setPost-java.lang.String-}
```
public void setPost(String value)
```


返回或设置用于通过 POST 方法向 Web 服务器输入数据以返回 Web 查询数据的字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


指定当连接失败时电子表格应用程序应执行的操作。默认值为 ReConnectionMethodType.Required。

参见 [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.ReconnectionMethodType 属性。此属性将在自 2017 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


指定当连接失败时电子表格应用程序应执行的操作。默认值为 ReConnectionMethodType.Required。

参见 [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


指定连接自动刷新之间的分钟数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


如果在打开文件时应刷新此连接则为 true；否则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSameSettings(boolean value) {#setSameSettings-boolean-}
```
public void setSameSettings(boolean value)
```


指示是否使用与第一行相同的宽度设置解析 PRE 块内所有表格的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


如果通过连接获取的用于填充表格的外部数据要随工作簿一起保存，则为 true；否则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


如果密码要作为连接字符串的一部分保存，则为 true；否则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


指定在使用数据透视表基于服务器的页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


当外部数据源基于文件时使用。如果此类数据源的连接失败，电子表格应用程序会尝试直接连接到该文件。可以使用 URI 或系统特定的文件路径表示法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


设置外部连接的数据源类型。

参见 [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextDates(boolean value) {#setTextDates-boolean-}
```
public void setTextDates(boolean value)
```


指示是否将日期作为文本而非日期导入工作表单元格的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置外部连接的数据源类型。

参见 [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype)。

**Remarks**

注意：此属性现已过时。请改用 ExternalConnection.SourceType 属性。此属性将在自 2024 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUrl(String value) {#setUrl-java.lang.String-}
```
public void setUrl(String value)
```


用于刷新外部数据的 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setXl2000(boolean value) {#setXl2000-boolean-}
```
public void setXl2000(boolean value)
```


此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询在 Microsoft Excel 2000 或更高版本的电子表格应用程序中刷新，则设置为 true。此为可选属性，可忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setXl97(boolean value) {#setXl97-boolean-}
```
public void setXl97(boolean value)
```


此标志用于向后兼容较旧的现有电子表格文件，如果此网络查询是在 Microsoft Excel 97 中创建的，则设置为 true。此为可选属性，可忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setXml(boolean value) {#setXml-boolean-}
```
public void setXml(boolean value)
```


如果网络查询源是 XML（而非 HTML），则为 true，否则为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setXmlSourceData(boolean value) {#setXmlSourceData-boolean-}
```
public void setXmlSourceData(boolean value)
```


指示应导入 XML 源数据而不是 HTML 表本身的标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

