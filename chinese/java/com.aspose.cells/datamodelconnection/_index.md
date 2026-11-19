---
title: "DataModelConnection"
second_title: "Aspose.Cells for Java API 参考"
description: "指定数据模型连接"
type: docs
url: /zh/java/com.aspose.cells/datamodelconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class DataModelConnection extends ExternalConnection
```

指定数据模型连接
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | 指示连接是否可以在后台（异步）刷新。 |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | 获取此 [ExternalConnection](../../com.aspose.cells/externalconnection) 对象的类型。 |
| [getCommand()](#getCommand--) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [getCommandType()](#getCommandType--) | 返回 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) 类型。 |
| [getConnectionDescription()](#getConnectionDescription--) | 指定此连接的用户描述 |
| [getConnectionFile()](#getConnectionFile--) | 获取连接文件。 |
| [getConnectionId()](#getConnectionId--) | 指定此连接的唯一标识符。 |
| [getConnectionString()](#getConnectionString--) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [getCredentials()](#getCredentials--) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [getId()](#getId--) | 获取连接的 ID。 |
| [getKeepAlive()](#getKeepAlive--) | 当电子表格应用程序应努力保持连接打开时为 true。 |
| [getName()](#getName--) | 指定连接的名称。 |
| [getOdcFile()](#getOdcFile--) | 指定创建此连接的外部连接文件的完整路径。 |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | 指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。 |
| [getParameters()](#getParameters--) | 获取用于 ODBC 或 Web 查询的 [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)。 |
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
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | 指示关联的工作簿连接是否已被删除。 |
| [isNew()](#isNew--) | 如果连接尚未首次刷新则为 true；否则为 false。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | 指示连接是否可以在后台（异步）刷新。 |
| [setCommand(String value)](#setCommand-java.lang.String-) | 包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据。 |
| [setCommandType(int value)](#setCommandType-int-) | 返回 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) 类型。 |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | 指定此连接的用户描述 |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。 |
| [setCredentials(int value)](#setCredentials-int-) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | 指定在建立（或重新建立）连接时使用的身份验证方法。 |
| [setDeleted(boolean value)](#setDeleted-boolean-) | 指示关联的工作簿连接是否已被删除。 |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | 当电子表格应用程序应努力保持连接打开时为 true。 |
| [setName(String value)](#setName-java.lang.String-) | 指定连接的名称。 |
| [setNew(boolean value)](#setNew-boolean-) | 如果连接尚未首次刷新则为 true；否则为 false。 |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | 指定创建此连接的外部连接文件的完整路径。 |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | 指示在刷新连接时，电子表格应用程序是否应始终且仅使用 odcFile 属性指示的外部连接文件中的连接信息。 |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | 指定当连接失败时，电子表格应用程序应执行的操作。 |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | 指定连接自动刷新之间的分钟数。 |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | 如果在打开文件时应刷新此连接则为 true；否则为 false。 |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | 用于在中间 spreadsheetML 服务器与外部数据源之间进行身份验证的单点登录 (SSO) 标识符。 |
| [setSaveData(boolean value)](#setSaveData-boolean-) | 如果通过连接获取的用于填充表格的外部数据要随工作簿一起保存，则为 true；否则为 false。 |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | 如果密码要作为连接字符串的一部分保存，则为 true；否则为 false。 |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | 指定在使用基于服务器的透视表页面字段时持久化的第二个命令文本字符串。 |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | 当外部数据源基于文件时使用。 |
| [setSourceType(int value)](#setSourceType-int-) | 设置外部连接的数据源类型。 |
| [setType(int value)](#setType-int-) | 设置外部连接的数据源类型。 |
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


返回 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) 类型。

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


指示关联的工作簿连接是否已被删除。若已删除则为 true；否则为 false。

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


如果连接尚未首次刷新则为 True；否则为 false。当用户在查询完成返回前保存文件时可能出现此状态。

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


返回 [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) 类型。

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

