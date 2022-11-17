---
title: ExternalConnection
second_title: Aspose.Cells for Java API Reference
description: Specifies an external data connection
type: docs
weight: 201
url: /java/com.aspose.cells/externalconnection/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExternalConnection
```

Specifies an external data connection
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indicates whether the connection can be refreshed in the background (asynchronously). |
| [getClass()](#getClass--) |  |
| [getConnectionDescription()](#getConnectionDescription--) | Specifies the user description for this connection |
| [getConnectionId()](#getConnectionId--) | Specifies The unique identifier of this connection. |
| [getCredentials()](#getCredentials--) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getId()](#getId--) | Gets the id of the connection. |
| [getKeepAlive()](#getKeepAlive--) | True when the spreadsheet application should make efforts to keep the connection open. |
| [getName()](#getName--) | Specifies the name of the connection. |
| [getOdcFile()](#getOdcFile--) | Specifies the full path to external connection file from which this connection was created. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. |
| [getParameters()](#getParameters--) | Gets [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) for an ODBC or web query. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Gets the definition of power query formula. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Specifies what the spreadsheet application should do when a connection fails. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Specifies what the spreadsheet application should do when a connection fails. |
| [getRefreshInternal()](#getRefreshInternal--) | Specifies the number of minutes between automatic refreshes of the connection. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [getSSOId()](#getSSOId--) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [getSaveData()](#getSaveData--) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [getSavePassword()](#getSavePassword--) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSourceFile()](#getSourceFile--) | Used when the external data source is file-based. |
| [getType()](#getType--) | Gets or Sets the external connection DataSource type. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Indicates whether the associated workbook connection has been deleted. |
| [isNew()](#isNew--) | True if the connection has not been refreshed for the first time; otherwise, false. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) |  |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) |  |
| [setCredentials(int value)](#setCredentials-int-) |  |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) |  |
| [setDeleted(boolean value)](#setDeleted-boolean-) |  |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) |  |
| [setName(String value)](#setName-java.lang.String-) |  |
| [setNew(boolean value)](#setNew-boolean-) |  |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) |  |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) |  |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) |  |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) |  |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) |  |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) |  |
| [setSSOId(String value)](#setSSOId-java.lang.String-) |  |
| [setSaveData(boolean value)](#setSaveData-boolean-) |  |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) |  |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) |  |
| [setType(int value)](#setType-int-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Specifies the user description for this connection

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Specifies The unique identifier of this connection.

**Returns:**
int
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Specifies the authentication method to be used when establishing (or re-establishing) the connection. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Specifies the authentication method to be used when establishing (or re-establishing) the connection.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Gets the id of the connection.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Specifies the name of the connection. Each connection must have a unique name.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Gets [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) for an ODBC or web query.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Gets the definition of power query formula.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Specifies the number of minutes between automatic refreshes of the connection.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


True if this connection should be refreshed when opening the file; otherwise, false.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


True if the password is to be saved as part of the connection string; otherwise, False.

**Returns:**
boolean
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Gets or Sets the external connection DataSource type.

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


Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

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




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

