##ExternalConnection Class
'ExternalConnection class. Encapsulates the object that represents externalconnection in Go.'
## ExternalConnection class
Specifies an external data connection
```go
type ExternalConnection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetId](./getid/) | Gets the id of the connection. |
|[GetSourceType](./getsourcetype/) | Gets or Sets the external connection DataSource type. |
|[SetSourceType](./setsourcetype/) | Gets or Sets the external connection DataSource type. |
|[GetSSOId](./getssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediatespreadsheetML server and the external data source. |
|[SetSSOId](./setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediatespreadsheetML server and the external data source. |
|[GetSavePassword](./getsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
|[SetSavePassword](./setsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
|[GetSaveData](./getsavedata/) | True if the external data fetched over the connection to populate a table is to be savedwith the workbook; otherwise, false. |
|[SetSaveData](./setsavedata/) | True if the external data fetched over the connection to populate a table is to be savedwith the workbook; otherwise, false. |
|[GetRefreshOnLoad](./getrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
|[SetRefreshOnLoad](./setrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
|[GetReconnectionMethodType](./getreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails.The default value is ReConnectionMethodType.Required. |
|[SetReconnectionMethodType](./setreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails.The default value is ReConnectionMethodType.Required. |
|[GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use theconnection information in the external connection file indicated by the odcFile attributewhen the connection is refreshed.  If false, then the spreadsheet applicationshould follow the procedure indicated by the reconnectionMethod attribute |
|[SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use theconnection information in the external connection file indicated by the odcFile attributewhen the connection is refreshed.  If false, then the spreadsheet applicationshould follow the procedure indicated by the reconnectionMethod attribute |
|[GetOdcFile](./getodcfile/) | Specifies the full path to external connection file from which this connection wascreated. If a connection fails during an attempt to refresh data, and reconnectionMethod=1,then the spreadsheet application will try again using information from the external connection fileinstead of the connection object embedded within the workbook. |
|[SetOdcFile](./setodcfile/) | Specifies the full path to external connection file from which this connection wascreated. If a connection fails during an attempt to refresh data, and reconnectionMethod=1,then the spreadsheet application will try again using information from the external connection fileinstead of the connection object embedded within the workbook. |
|[GetSourceFile](./getsourcefile/) | Used when the external data source is file-based.When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May beexpressed in URI or system-specific file path notation. |
|[SetSourceFile](./setsourcefile/) | Used when the external data source is file-based.When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May beexpressed in URI or system-specific file path notation. |
|[IsNew](./isnew/) | True if the connection has not been refreshed for the first time; otherwise, false.This state can happen when the user saves the file before a query has finished returning. |
|[SetIsNew](./setisnew/) | True if the connection has not been refreshed for the first time; otherwise, false.This state can happen when the user saves the file before a query has finished returning. |
|[GetName](./getname/) | Specifies the name of the connection. Each connection must have a unique name. |
|[SetName](./setname/) | Specifies the name of the connection. Each connection must have a unique name. |
|[GetKeepAlive](./getkeepalive/) | True when the spreadsheet application should make efforts to keep the connectionopen. When false, the application should close the connection after retrieving theinformation. |
|[SetKeepAlive](./setkeepalive/) | True when the spreadsheet application should make efforts to keep the connectionopen. When false, the application should close the connection after retrieving theinformation. |
|[GetRefreshInternal](./getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
|[SetRefreshInternal](./setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
|[GetConnectionDescription](./getconnectiondescription/) | Specifies the user description for this connection |
|[SetConnectionDescription](./setconnectiondescription/) | Specifies the user description for this connection |
|[IsDeleted](./isdeleted/) | Indicates whether the associated workbook connection has been deleted.  true if theconnection has been deleted; otherwise, false. |
|[SetIsDeleted](./setisdeleted/) | Indicates whether the associated workbook connection has been deleted.  true if theconnection has been deleted; otherwise, false. |
|[GetCredentialsMethodType](./getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
|[SetCredentialsMethodType](./setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
|[GetBackgroundRefresh](./getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously).true if preferred usage of the connection is to refresh asynchronously in the background;false if preferred usage of the connection is to refresh synchronously in the foreground. |
|[SetBackgroundRefresh](./setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously).true if preferred usage of the connection is to refresh asynchronously in the background;false if preferred usage of the connection is to refresh synchronously in the foreground. |
|[GetParameters](./getparameters/) | Gets ConnectionParameterCollection for an ODBC or web query. |
|[GetClassType](./getclasstype/) | Gets the type of this ExternalConnection object. |
|[GetPowerQueryFormula](./getpowerqueryformula/) | Gets the definition of power query formula. |
|[GetConnectionFile](./getconnectionfile/) | Gets the connection file. |
|[GetCommand](./getcommand/) | The string containing the database command to pass to the data provider API that willinteract with the external source in order to retrieve data |
|[SetCommand](./setcommand/) | The string containing the database command to pass to the data provider API that willinteract with the external source in order to retrieve data |
|[GetCommandType](./getcommandtype/) | Specifies the OLE DB command type.1. Query specifies a cube name2. Query specifies a SQL statement3. Query specifies a table name4. Query specifies that default information has been given, and it is up to the provider how to interpret.5. Query is against a web based List Data Provider. |
|[SetCommandType](./setcommandtype/) | Specifies the OLE DB command type.1. Query specifies a cube name2. Query specifies a SQL statement3. Query specifies a table name4. Query specifies that default information has been given, and it is up to the provider how to interpret.5. Query is against a web based List Data Provider. |
|[GetConnectionString](./getconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
|[SetConnectionString](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
|[GetSecondCommand](./getsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed |
|[SetSecondCommand](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed |
