---
title: DBConnection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies all properties associated with an ODBC or OLE DB external data connection.
type: docs
url: /nodejs-cpp/dbconnection/
---

## DBConnection class

Specifies all properties associated with an ODBC or OLE DB external data connection.

```javascript
class DBConnection extends ExternalConnection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ExternalConnection)](#constructor-externalconnection-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getClassType()](#getClassType--)| Gets the type of this [ExternalConnection](../externalconnection/) object. |
| [getConnectionString()](#getConnectionString--)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionString(string)](#setConnectionString-string-)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getConnectionInfo()](#getConnectionInfo--)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionInfo(string)](#setConnectionInfo-string-)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getPowerQueryFormula()](#getPowerQueryFormula--)| Gets the definition of power query formula. |
| [getCommandType()](#getCommandType--)| Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. |
| [setCommandType(OLEDBCommandType)](#setCommandType-oledbcommandtype-)| Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. |
| [getCommand()](#getCommand--)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [setCommand(string)](#setCommand-string-)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [getSeverCommand()](#getSeverCommand--)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [setSeverCommand(string)](#setSeverCommand-string-)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [getSecondCommand()](#getSecondCommand--)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [setSecondCommand(string)](#setSecondCommand-string-)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getId()](#getId--)| Gets the id of the connection. |
| [getConnectionId()](#getConnectionId--)| Specifies The unique identifier of this connection. |
| [getSourceType()](#getSourceType--)| Gets or Sets the external connection DataSource type. |
| [setSourceType(ConnectionDataSourceType)](#setSourceType-connectiondatasourcetype-)| Gets or Sets the external connection DataSource type. |
| [getSSOId()](#getSSOId--)| Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [setSSOId(string)](#setSSOId-string-)| Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [getSavePassword()](#getSavePassword--)| True if the password is to be saved as part of the connection string; otherwise, False. |
| [setSavePassword(boolean)](#setSavePassword-boolean-)| True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSaveData()](#getSaveData--)| True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [setSaveData(boolean)](#setSaveData-boolean-)| True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [getRefreshOnLoad()](#getRefreshOnLoad--)| True if this connection should be refreshed when opening the file; otherwise, false. |
| [setRefreshOnLoad(boolean)](#setRefreshOnLoad-boolean-)| True if this connection should be refreshed when opening the file; otherwise, false. |
| [getReconnectionMethodType()](#getReconnectionMethodType--)| Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [setReconnectionMethodType(ReConnectionMethodType)](#setReconnectionMethodType-reconnectionmethodtype-)| Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--)| Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [setOnlyUseConnectionFile(boolean)](#setOnlyUseConnectionFile-boolean-)| Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [getOdcFile()](#getOdcFile--)| Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [setOdcFile(string)](#setOdcFile-string-)| Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [getSourceFile()](#getSourceFile--)| Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [setSourceFile(string)](#setSourceFile-string-)| Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [isNew()](#isNew--)| True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [setIsNew(boolean)](#setIsNew-boolean-)| True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [getName()](#getName--)| Specifies the name of the connection. Each connection must have a unique name. |
| [setName(string)](#setName-string-)| Specifies the name of the connection. Each connection must have a unique name. |
| [getKeepAlive()](#getKeepAlive--)| True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [setKeepAlive(boolean)](#setKeepAlive-boolean-)| True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [getRefreshInternal()](#getRefreshInternal--)| Specifies the number of minutes between automatic refreshes of the connection. |
| [setRefreshInternal(number)](#setRefreshInternal-number-)| Specifies the number of minutes between automatic refreshes of the connection. |
| [getConnectionDescription()](#getConnectionDescription--)| Specifies the user description for this connection |
| [setConnectionDescription(string)](#setConnectionDescription-string-)| Specifies the user description for this connection |
| [isDeleted()](#isDeleted--)| Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [getCredentialsMethodType()](#getCredentialsMethodType--)| Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [setCredentialsMethodType(CredentialsMethodType)](#setCredentialsMethodType-credentialsmethodtype-)| Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getBackgroundRefresh()](#getBackgroundRefresh--)| Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [setBackgroundRefresh(boolean)](#setBackgroundRefresh-boolean-)| Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [getParameters()](#getParameters--)| Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
| [getConnectionFile()](#getConnectionFile--)| Gets the connection file. |


### constructor(ExternalConnection) {#constructor-externalconnection-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ExternalConnection);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ExternalConnection | The parent object. |

### getClassType() {#getClassType--}

Gets the type of this [ExternalConnection](../externalconnection/) object.

```javascript
getClassType() : ExternalConnectionClassType;
```


**Returns**

[ExternalConnectionClassType](../externalconnectionclasstype/)

### getConnectionString() {#getConnectionString--}

The connection information string is used to make contact with an OLE DB or ODBC data source.

```javascript
getConnectionString() : string;
```


### setConnectionString(string) {#setConnectionString-string-}

The connection information string is used to make contact with an OLE DB or ODBC data source.

```javascript
setConnectionString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getConnectionInfo() {#getConnectionInfo--}

The connection information string is used to make contact with an OLE DB or ODBC data source.

```javascript
getConnectionInfo() : string;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### setConnectionInfo(string) {#setConnectionInfo-string-}

The connection information string is used to make contact with an OLE DB or ODBC data source.

```javascript
setConnectionInfo(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### getPowerQueryFormula() {#getPowerQueryFormula--}

Gets the definition of power query formula.

```javascript
getPowerQueryFormula() : PowerQueryFormula;
```


**Returns**

[PowerQueryFormula](../powerqueryformula/)

### getCommandType() {#getCommandType--}

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.

```javascript
getCommandType() : OLEDBCommandType;
```


**Returns**

[OLEDBCommandType](../oledbcommandtype/)

### setCommandType(OLEDBCommandType) {#setCommandType-oledbcommandtype-}

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.

```javascript
setCommandType(value: OLEDBCommandType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OLEDBCommandType](../oledbcommandtype/) | The value to set. |

### getCommand() {#getCommand--}

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

```javascript
getCommand() : string;
```


### setCommand(string) {#setCommand-string-}

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

```javascript
setCommand(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSeverCommand() {#getSeverCommand--}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```javascript
getSeverCommand() : string;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### setSeverCommand(string) {#setSeverCommand-string-}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```javascript
setSeverCommand(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### getSecondCommand() {#getSecondCommand--}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```javascript
getSecondCommand() : string;
```


### setSecondCommand(string) {#setSecondCommand-string-}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```javascript
setSecondCommand(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getId() {#getId--}

Gets the id of the connection.

```javascript
getId() : number;
```


### getConnectionId() {#getConnectionId--}

Specifies The unique identifier of this connection.

```javascript
getConnectionId() : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ExternalConnection.Id property. This property will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### getSourceType() {#getSourceType--}

Gets or Sets the external connection DataSource type.

```javascript
getSourceType() : ConnectionDataSourceType;
```


**Returns**

[ConnectionDataSourceType](../connectiondatasourcetype/)

### setSourceType(ConnectionDataSourceType) {#setSourceType-connectiondatasourcetype-}

Gets or Sets the external connection DataSource type.

```javascript
setSourceType(value: ConnectionDataSourceType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionDataSourceType](../connectiondatasourcetype/) | The value to set. |

### getSSOId() {#getSSOId--}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

```javascript
getSSOId() : string;
```


### setSSOId(string) {#setSSOId-string-}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

```javascript
setSSOId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSavePassword() {#getSavePassword--}

True if the password is to be saved as part of the connection string; otherwise, False.

```javascript
getSavePassword() : boolean;
```


### setSavePassword(boolean) {#setSavePassword-boolean-}

True if the password is to be saved as part of the connection string; otherwise, False.

```javascript
setSavePassword(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSaveData() {#getSaveData--}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

```javascript
getSaveData() : boolean;
```


### setSaveData(boolean) {#setSaveData-boolean-}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

```javascript
setSaveData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshOnLoad() {#getRefreshOnLoad--}

True if this connection should be refreshed when opening the file; otherwise, false.

```javascript
getRefreshOnLoad() : boolean;
```


### setRefreshOnLoad(boolean) {#setRefreshOnLoad-boolean-}

True if this connection should be refreshed when opening the file; otherwise, false.

```javascript
setRefreshOnLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReconnectionMethodType() {#getReconnectionMethodType--}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

```javascript
getReconnectionMethodType() : ReConnectionMethodType;
```


**Returns**

[ReConnectionMethodType](../reconnectionmethodtype/)

### setReconnectionMethodType(ReConnectionMethodType) {#setReconnectionMethodType-reconnectionmethodtype-}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

```javascript
setReconnectionMethodType(value: ReConnectionMethodType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReConnectionMethodType](../reconnectionmethodtype/) | The value to set. |

### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

```javascript
getOnlyUseConnectionFile() : boolean;
```


### setOnlyUseConnectionFile(boolean) {#setOnlyUseConnectionFile-boolean-}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

```javascript
setOnlyUseConnectionFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOdcFile() {#getOdcFile--}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

```javascript
getOdcFile() : string;
```


### setOdcFile(string) {#setOdcFile-string-}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

```javascript
setOdcFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSourceFile() {#getSourceFile--}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

```javascript
getSourceFile() : string;
```


### setSourceFile(string) {#setSourceFile-string-}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

```javascript
setSourceFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isNew() {#isNew--}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

```javascript
isNew() : boolean;
```


### setIsNew(boolean) {#setIsNew-boolean-}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

```javascript
setIsNew(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getName() {#getName--}

Specifies the name of the connection. Each connection must have a unique name.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Specifies the name of the connection. Each connection must have a unique name.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getKeepAlive() {#getKeepAlive--}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

```javascript
getKeepAlive() : boolean;
```


### setKeepAlive(boolean) {#setKeepAlive-boolean-}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

```javascript
setKeepAlive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshInternal() {#getRefreshInternal--}

Specifies the number of minutes between automatic refreshes of the connection.

```javascript
getRefreshInternal() : number;
```


### setRefreshInternal(number) {#setRefreshInternal-number-}

Specifies the number of minutes between automatic refreshes of the connection.

```javascript
setRefreshInternal(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getConnectionDescription() {#getConnectionDescription--}

Specifies the user description for this connection

```javascript
getConnectionDescription() : string;
```


### setConnectionDescription(string) {#setConnectionDescription-string-}

Specifies the user description for this connection

```javascript
setConnectionDescription(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isDeleted() {#isDeleted--}

Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false.

```javascript
isDeleted() : boolean;
```


### setIsDeleted(boolean) {#setIsDeleted-boolean-}

Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false.

```javascript
setIsDeleted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCredentialsMethodType() {#getCredentialsMethodType--}

Specifies the authentication method to be used when establishing (or re-establishing) the connection.

```javascript
getCredentialsMethodType() : CredentialsMethodType;
```


**Returns**

[CredentialsMethodType](../credentialsmethodtype/)

### setCredentialsMethodType(CredentialsMethodType) {#setCredentialsMethodType-credentialsmethodtype-}

Specifies the authentication method to be used when establishing (or re-establishing) the connection.

```javascript
setCredentialsMethodType(value: CredentialsMethodType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CredentialsMethodType](../credentialsmethodtype/) | The value to set. |

### getBackgroundRefresh() {#getBackgroundRefresh--}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

```javascript
getBackgroundRefresh() : boolean;
```


### setBackgroundRefresh(boolean) {#setBackgroundRefresh-boolean-}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

```javascript
setBackgroundRefresh(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getParameters() {#getParameters--}

Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query.

```javascript
getParameters() : ConnectionParameterCollection;
```


**Returns**

[ConnectionParameterCollection](../connectionparametercollection/)

### getConnectionFile() {#getConnectionFile--}

Gets the connection file.

```javascript
getConnectionFile() : string;
```



