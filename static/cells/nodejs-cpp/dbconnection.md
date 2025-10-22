##DBConnection
Specifies all properties associated with an ODBC or OLE DB external data connection.
## DBConnection class
Specifies all properties associated with an ODBC or OLE DB external data connection.
```javascript
class DBConnection extends ExternalConnection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(ExternalConnection)](#constructor-externalconnection-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [connectionInfo](#connectionInfo--)| string | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [severCommand](#severCommand--)| string | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [id](#id--)| number | Readonly. Gets the id of the connection. |
| [connectionId](#connectionId--)| number | Readonly. Specifies The unique identifier of this connection. |
| [sourceType](#sourceType--)| ConnectionDataSourceType | Gets or Sets the external connection DataSource type. |
| [sSOId](#sSOId--)| string | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [savePassword](#savePassword--)| boolean | True if the password is to be saved as part of the connection string; otherwise, False. |
| [saveData](#saveData--)| boolean | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [refreshOnLoad](#refreshOnLoad--)| boolean | True if this connection should be refreshed when opening the file; otherwise, false. |
| [reconnectionMethodType](#reconnectionMethodType--)| ReConnectionMethodType | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [onlyUseConnectionFile](#onlyUseConnectionFile--)| boolean | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [odcFile](#odcFile--)| string | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [sourceFile](#sourceFile--)| string | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [isNew](#isNew--)| boolean | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [name](#name--)| string | Specifies the name of the connection. Each connection must have a unique name. |
| [keepAlive](#keepAlive--)| boolean | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [refreshInternal](#refreshInternal--)| number | Specifies the number of minutes between automatic refreshes of the connection. |
| [connectionDescription](#connectionDescription--)| string | Specifies the user description for this connection |
| [isDeleted](#isDeleted--)| boolean | Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [credentialsMethodType](#credentialsMethodType--)| CredentialsMethodType | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [backgroundRefresh](#backgroundRefresh--)| boolean | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [parameters](#parameters--)| ConnectionParameterCollection | Readonly. Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
## Methods
| Method | Description |
| --- | --- |
| [getConnectionInfo()](#getConnectionInfo--)| <b>@deprecated.</b> Please use the 'connectionInfo' property instead. The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionInfo(string)](#setConnectionInfo-string-)| <b>@deprecated.</b> Please use the 'connectionInfo' property instead. The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getSeverCommand()](#getSeverCommand--)| <b>@deprecated.</b> Please use the 'severCommand' property instead. Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [setSeverCommand(string)](#setSeverCommand-string-)| <b>@deprecated.</b> Please use the 'severCommand' property instead. Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the id of the connection. |
| [getConnectionId()](#getConnectionId--)| <b>@deprecated.</b> Please use the 'connectionId' property instead. Specifies The unique identifier of this connection. |
| [getSourceType()](#getSourceType--)| <b>@deprecated.</b> Please use the 'sourceType' property instead. Gets or Sets the external connection DataSource type. |
| [setSourceType(ConnectionDataSourceType)](#setSourceType-connectiondatasourcetype-)| <b>@deprecated.</b> Please use the 'sourceType' property instead. Gets or Sets the external connection DataSource type. |
| [getSSOId()](#getSSOId--)| <b>@deprecated.</b> Please use the 'sSOId' property instead. Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [setSSOId(string)](#setSSOId-string-)| <b>@deprecated.</b> Please use the 'sSOId' property instead. Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [getSavePassword()](#getSavePassword--)| <b>@deprecated.</b> Please use the 'savePassword' property instead. True if the password is to be saved as part of the connection string; otherwise, False. |
| [setSavePassword(boolean)](#setSavePassword-boolean-)| <b>@deprecated.</b> Please use the 'savePassword' property instead. True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSaveData()](#getSaveData--)| <b>@deprecated.</b> Please use the 'saveData' property instead. True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [setSaveData(boolean)](#setSaveData-boolean-)| <b>@deprecated.</b> Please use the 'saveData' property instead. True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [getRefreshOnLoad()](#getRefreshOnLoad--)| <b>@deprecated.</b> Please use the 'refreshOnLoad' property instead. True if this connection should be refreshed when opening the file; otherwise, false. |
| [setRefreshOnLoad(boolean)](#setRefreshOnLoad-boolean-)| <b>@deprecated.</b> Please use the 'refreshOnLoad' property instead. True if this connection should be refreshed when opening the file; otherwise, false. |
| [getReconnectionMethodType()](#getReconnectionMethodType--)| <b>@deprecated.</b> Please use the 'reconnectionMethodType' property instead. Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [setReconnectionMethodType(ReConnectionMethodType)](#setReconnectionMethodType-reconnectionmethodtype-)| <b>@deprecated.</b> Please use the 'reconnectionMethodType' property instead. Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--)| <b>@deprecated.</b> Please use the 'onlyUseConnectionFile' property instead. Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [setOnlyUseConnectionFile(boolean)](#setOnlyUseConnectionFile-boolean-)| <b>@deprecated.</b> Please use the 'onlyUseConnectionFile' property instead. Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [getOdcFile()](#getOdcFile--)| <b>@deprecated.</b> Please use the 'odcFile' property instead. Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [setOdcFile(string)](#setOdcFile-string-)| <b>@deprecated.</b> Please use the 'odcFile' property instead. Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [getSourceFile()](#getSourceFile--)| <b>@deprecated.</b> Please use the 'sourceFile' property instead. Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [setSourceFile(string)](#setSourceFile-string-)| <b>@deprecated.</b> Please use the 'sourceFile' property instead. Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [isNew()](#isNew--)| <b>@deprecated.</b> Please use the 'isNew' property instead. True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [setIsNew(boolean)](#setIsNew-boolean-)| <b>@deprecated.</b> Please use the 'isNew' property instead. True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Specifies the name of the connection. Each connection must have a unique name. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Specifies the name of the connection. Each connection must have a unique name. |
| [getKeepAlive()](#getKeepAlive--)| <b>@deprecated.</b> Please use the 'keepAlive' property instead. True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [setKeepAlive(boolean)](#setKeepAlive-boolean-)| <b>@deprecated.</b> Please use the 'keepAlive' property instead. True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [getRefreshInternal()](#getRefreshInternal--)| <b>@deprecated.</b> Please use the 'refreshInternal' property instead. Specifies the number of minutes between automatic refreshes of the connection. |
| [setRefreshInternal(number)](#setRefreshInternal-number-)| <b>@deprecated.</b> Please use the 'refreshInternal' property instead. Specifies the number of minutes between automatic refreshes of the connection. |
| [getConnectionDescription()](#getConnectionDescription--)| <b>@deprecated.</b> Please use the 'connectionDescription' property instead. Specifies the user description for this connection |
| [setConnectionDescription(string)](#setConnectionDescription-string-)| <b>@deprecated.</b> Please use the 'connectionDescription' property instead. Specifies the user description for this connection |
| [isDeleted()](#isDeleted--)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [getCredentialsMethodType()](#getCredentialsMethodType--)| <b>@deprecated.</b> Please use the 'credentialsMethodType' property instead. Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [setCredentialsMethodType(CredentialsMethodType)](#setCredentialsMethodType-credentialsmethodtype-)| <b>@deprecated.</b> Please use the 'credentialsMethodType' property instead. Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getBackgroundRefresh()](#getBackgroundRefresh--)| <b>@deprecated.</b> Please use the 'backgroundRefresh' property instead. Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [setBackgroundRefresh(boolean)](#setBackgroundRefresh-boolean-)| <b>@deprecated.</b> Please use the 'backgroundRefresh' property instead. Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [getParameters()](#getParameters--)| <b>@deprecated.</b> Please use the 'parameters' property instead. Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
| [getClassType()](#getClassType--)| Gets the type of this [ExternalConnection](../externalconnection/) object. |
| [getConnectionString()](#getConnectionString--)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionString(string)](#setConnectionString-string-)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getPowerQueryFormula()](#getPowerQueryFormula--)| Gets the definition of power query formula. |
| [getCommandType()](#getCommandType--)| Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. |
| [setCommandType(OLEDBCommandType)](#setCommandType-oledbcommandtype-)| Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. |
| [getCommand()](#getCommand--)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [setCommand(string)](#setCommand-string-)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [getSecondCommand()](#getSecondCommand--)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [setSecondCommand(string)](#setSecondCommand-string-)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
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
### connectionInfo {#connectionInfo--}
The connection information string is used to make contact with an OLE DB or ODBC data source.
```javascript
connectionInfo : string;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### severCommand {#severCommand--}
Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed
```javascript
severCommand : string;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### id {#id--}
Readonly. Gets the id of the connection.
```javascript
id : number;
```
### connectionId {#connectionId--}
Readonly. Specifies The unique identifier of this connection.
```javascript
connectionId : number;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.Id property. This property will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### sourceType {#sourceType--}
Gets or Sets the external connection DataSource type.
```javascript
sourceType : ConnectionDataSourceType;
```
### sSOId {#sSOId--}
Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.
```javascript
sSOId : string;
```
### savePassword {#savePassword--}
True if the password is to be saved as part of the connection string; otherwise, False.
```javascript
savePassword : boolean;
```
### saveData {#saveData--}
True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.
```javascript
saveData : boolean;
```
### refreshOnLoad {#refreshOnLoad--}
True if this connection should be refreshed when opening the file; otherwise, false.
```javascript
refreshOnLoad : boolean;
```
### reconnectionMethodType {#reconnectionMethodType--}
Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.
```javascript
reconnectionMethodType : ReConnectionMethodType;
```
### onlyUseConnectionFile {#onlyUseConnectionFile--}
Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute
```javascript
onlyUseConnectionFile : boolean;
```
### odcFile {#odcFile--}
Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.
```javascript
odcFile : string;
```
### sourceFile {#sourceFile--}
Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.
```javascript
sourceFile : string;
```
### isNew {#isNew--}
True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.
```javascript
isNew : boolean;
```
### name {#name--}
Specifies the name of the connection. Each connection must have a unique name.
```javascript
name : string;
```
### keepAlive {#keepAlive--}
True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.
```javascript
keepAlive : boolean;
```
### refreshInternal {#refreshInternal--}
Specifies the number of minutes between automatic refreshes of the connection.
```javascript
refreshInternal : number;
```
### connectionDescription {#connectionDescription--}
Specifies the user description for this connection
```javascript
connectionDescription : string;
```
### isDeleted {#isDeleted--}
Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false.
```javascript
isDeleted : boolean;
```
### credentialsMethodType {#credentialsMethodType--}
Specifies the authentication method to be used when establishing (or re-establishing) the connection.
```javascript
credentialsMethodType : CredentialsMethodType;
```
### backgroundRefresh {#backgroundRefresh--}
Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.
```javascript
backgroundRefresh : boolean;
```
### parameters {#parameters--}
Readonly. Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query.
```javascript
parameters : ConnectionParameterCollection;
```
### getConnectionInfo() {#getConnectionInfo--}
```javascript
getConnectionInfo() : string;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### setConnectionInfo(string) {#setConnectionInfo-string-}
```javascript
setConnectionInfo(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### getSeverCommand() {#getSeverCommand--}
```javascript
getSeverCommand() : string;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### setSeverCommand(string) {#setSeverCommand-string-}
```javascript
setSeverCommand(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getId() {#getId--}
```javascript
getId() : number;
```
### getConnectionId() {#getConnectionId--}
```javascript
getConnectionId() : number;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use ExternalConnection.Id property. This property will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### getSourceType() {#getSourceType--}
```javascript
getSourceType() : ConnectionDataSourceType;
```
**Returns**
[ConnectionDataSourceType](../connectiondatasourcetype/)
### setSourceType(ConnectionDataSourceType) {#setSourceType-connectiondatasourcetype-}
```javascript
setSourceType(value: ConnectionDataSourceType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionDataSourceType](../connectiondatasourcetype/) | The value to set. |
### getSSOId() {#getSSOId--}
```javascript
getSSOId() : string;
```
### setSSOId(string) {#setSSOId-string-}
```javascript
setSSOId(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSavePassword() {#getSavePassword--}
```javascript
getSavePassword() : boolean;
```
### setSavePassword(boolean) {#setSavePassword-boolean-}
```javascript
setSavePassword(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSaveData() {#getSaveData--}
```javascript
getSaveData() : boolean;
```
### setSaveData(boolean) {#setSaveData-boolean-}
```javascript
setSaveData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshOnLoad() {#getRefreshOnLoad--}
```javascript
getRefreshOnLoad() : boolean;
```
### setRefreshOnLoad(boolean) {#setRefreshOnLoad-boolean-}
```javascript
setRefreshOnLoad(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getReconnectionMethodType() {#getReconnectionMethodType--}
```javascript
getReconnectionMethodType() : ReConnectionMethodType;
```
**Returns**
[ReConnectionMethodType](../reconnectionmethodtype/)
### setReconnectionMethodType(ReConnectionMethodType) {#setReconnectionMethodType-reconnectionmethodtype-}
```javascript
setReconnectionMethodType(value: ReConnectionMethodType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReConnectionMethodType](../reconnectionmethodtype/) | The value to set. |
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```javascript
getOnlyUseConnectionFile() : boolean;
```
### setOnlyUseConnectionFile(boolean) {#setOnlyUseConnectionFile-boolean-}
```javascript
setOnlyUseConnectionFile(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOdcFile() {#getOdcFile--}
```javascript
getOdcFile() : string;
```
### setOdcFile(string) {#setOdcFile-string-}
```javascript
setOdcFile(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSourceFile() {#getSourceFile--}
```javascript
getSourceFile() : string;
```
### setSourceFile(string) {#setSourceFile-string-}
```javascript
setSourceFile(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNew() {#isNew--}
```javascript
isNew() : boolean;
```
### setIsNew(boolean) {#setIsNew-boolean-}
```javascript
setIsNew(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getKeepAlive() {#getKeepAlive--}
```javascript
getKeepAlive() : boolean;
```
### setKeepAlive(boolean) {#setKeepAlive-boolean-}
```javascript
setKeepAlive(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshInternal() {#getRefreshInternal--}
```javascript
getRefreshInternal() : number;
```
### setRefreshInternal(number) {#setRefreshInternal-number-}
```javascript
setRefreshInternal(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getConnectionDescription() {#getConnectionDescription--}
```javascript
getConnectionDescription() : string;
```
### setConnectionDescription(string) {#setConnectionDescription-string-}
```javascript
setConnectionDescription(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isDeleted() {#isDeleted--}
```javascript
isDeleted() : boolean;
```
### setIsDeleted(boolean) {#setIsDeleted-boolean-}
```javascript
setIsDeleted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCredentialsMethodType() {#getCredentialsMethodType--}
```javascript
getCredentialsMethodType() : CredentialsMethodType;
```
**Returns**
[CredentialsMethodType](../credentialsmethodtype/)
### setCredentialsMethodType(CredentialsMethodType) {#setCredentialsMethodType-credentialsmethodtype-}
```javascript
setCredentialsMethodType(value: CredentialsMethodType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CredentialsMethodType](../credentialsmethodtype/) | The value to set. |
### getBackgroundRefresh() {#getBackgroundRefresh--}
```javascript
getBackgroundRefresh() : boolean;
```
### setBackgroundRefresh(boolean) {#setBackgroundRefresh-boolean-}
```javascript
setBackgroundRefresh(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getParameters() {#getParameters--}
```javascript
getParameters() : ConnectionParameterCollection;
```
**Returns**
[ConnectionParameterCollection](../connectionparametercollection/)
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
### getConnectionFile() {#getConnectionFile--}
Gets the connection file.
```javascript
getConnectionFile() : string;
```
