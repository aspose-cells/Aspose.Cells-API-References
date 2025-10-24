##Aspose::Cells::ExternalConnections::ExternalConnection class
'Aspose::Cells::ExternalConnections::ExternalConnection class. Specifies an external data connection in C++.'
## ExternalConnection class
Specifies an external data connection.
```cpp
class ExternalConnection
```
## Methods
| Method | Description |
| --- | --- |
| [ExternalConnection(ExternalConnection_Impl* impl)](./externalconnection/) | Constructs from an implementation object. |
| [ExternalConnection(const ExternalConnection\& src)](./externalconnection/) | Copy constructor. |
| [GetBackgroundRefresh()](./getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| virtual [GetClassType()](./getclasstype/) | Gets the type of this [ExternalConnection](./) object. |
| [GetCommand()](./getcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [GetCommandType()](./getcommandtype/) | Specifies the OLE DB command type. |
| [GetConnectionDescription()](./getconnectiondescription/) | Specifies the user description for this connection. |
| [GetConnectionFile()](./getconnectionfile/) | Gets the connection file. |
| [GetConnectionId()](./getconnectionid/) |  **(Deprecated)** Specifies The unique identifier of this connection. |
| [GetConnectionString()](./getconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [GetCredentialsMethodType()](./getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [GetId()](./getid/) | Gets the id of the connection. |
| [GetKeepAlive()](./getkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [GetName()](./getname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [GetOdcFile()](./getodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [GetOnlyUseConnectionFile()](./getonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [GetParameters()](./getparameters/) | Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
| [GetPowerQueryFormula()](./getpowerqueryformula/) | Gets the definition of power query formula. |
| [GetReconnectionMethodType()](./getreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [GetRefreshInternal()](./getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [GetRefreshOnLoad()](./getrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [GetSaveData()](./getsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [GetSavePassword()](./getsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [GetSecondCommand()](./getsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [GetSourceFile()](./getsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [GetSourceType()](./getsourcetype/) | Gets or Sets the external connection DataSource type. |
| [GetSSOId()](./getssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [IsDeleted()](./isdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [IsNew()](./isnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ExternalConnection\& src)](./operator_asm/) | operator= |
| [SetBackgroundRefresh(bool value)](./setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [SetCommand(const U16String\& value)](./setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommand(const char16_t* value)](./setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommandType(OLEDBCommandType value)](./setcommandtype/) | Specifies the OLE DB command type. |
| [SetConnectionDescription(const U16String\& value)](./setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionDescription(const char16_t* value)](./setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionString(const U16String\& value)](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetConnectionString(const char16_t* value)](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetCredentialsMethodType(CredentialsMethodType value)](./setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [SetIsDeleted(bool value)](./setisdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [SetIsNew(bool value)](./setisnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [SetKeepAlive(bool value)](./setkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [SetName(const U16String\& value)](./setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetName(const char16_t* value)](./setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetOdcFile(const U16String\& value)](./setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOdcFile(const char16_t* value)](./setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOnlyUseConnectionFile(bool value)](./setonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [SetReconnectionMethodType(ReConnectionMethodType value)](./setreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [SetRefreshInternal(int32_t value)](./setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [SetRefreshOnLoad(bool value)](./setrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [SetSaveData(bool value)](./setsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [SetSavePassword(bool value)](./setsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SetSecondCommand(const U16String\& value)](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSecondCommand(const char16_t* value)](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSourceFile(const U16String\& value)](./setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceFile(const char16_t* value)](./setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceType(ConnectionDataSourceType value)](./setsourcetype/) | Gets or Sets the external connection DataSource type. |
| [SetSSOId(const U16String\& value)](./setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [SetSSOId(const char16_t* value)](./setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [~ExternalConnection()](./~externalconnection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
