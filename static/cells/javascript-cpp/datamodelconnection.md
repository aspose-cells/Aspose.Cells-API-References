##DataModelConnection
Specifies a data model connection
## DataModelConnection class
Specifies a data model connection
```javascript
class DataModelConnection extends ExternalConnection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(ExternalConnection)](#constructor-externalconnection-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
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
| [getClassType()](#getClassType--)| Gets the type of this [ExternalConnection](../externalconnection/) object. |
| [getCommand()](#getCommand--)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [setCommand(string)](#setCommand-string-)| The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| [getCommandType()](#getCommandType--)| Returns [OLEDBCommandType](../oledbcommandtype/) type. |
| [setCommandType(OLEDBCommandType)](#setCommandType-oledbcommandtype-)| Returns [OLEDBCommandType](../oledbcommandtype/) type. |
| [getConnectionString()](#getConnectionString--)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionString(string)](#setConnectionString-string-)| The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getPowerQueryFormula()](#getPowerQueryFormula--)| Gets the definition of power query formula. |
| [getConnectionFile()](#getConnectionFile--)| Gets the connection file. |
| [getSecondCommand()](#getSecondCommand--)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [setSecondCommand(string)](#setSecondCommand-string-)| Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
### constructor(ExternalConnection) {#constructor-externalconnection-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: ExternalConnection);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ExternalConnection | The parent object. |
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
### getClassType() {#getClassType--}
Gets the type of this [ExternalConnection](../externalconnection/) object.
```javascript
getClassType() : ExternalConnectionClassType;
```
**Returns**
[ExternalConnectionClassType](../externalconnectionclasstype/)
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
### getCommandType() {#getCommandType--}
Returns [OLEDBCommandType](../oledbcommandtype/) type.
```javascript
getCommandType() : OLEDBCommandType;
```
**Returns**
[OLEDBCommandType](../oledbcommandtype/)
### setCommandType(OLEDBCommandType) {#setCommandType-oledbcommandtype-}
Returns [OLEDBCommandType](../oledbcommandtype/) type.
```javascript
setCommandType(value: OLEDBCommandType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OLEDBCommandType](../oledbcommandtype/) | The value to set. |
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
### getConnectionFile() {#getConnectionFile--}
Gets the connection file.
```javascript
getConnectionFile() : string;
```
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
