##Aspose::Cells::ExternalConnections::DBConnection class
'Aspose::Cells::ExternalConnections::DBConnection class. Specifies all properties associated with an ODBC or OLE DB external data connection in C++.'
## DBConnection class
Specifies all properties associated with an ODBC or OLE DB external data connection.
```cpp
class DBConnection : public Aspose::Cells::ExternalConnections::ExternalConnection
```
## Methods
| Method | Description |
| --- | --- |
| [DBConnection(DBConnection_Impl* impl)](./dbconnection/) | Constructs from an implementation object. |
| [DBConnection(const DBConnection\& src)](./dbconnection/) | Copy constructor. |
| [DBConnection(const ExternalConnection\& src)](./dbconnection/) | Constructs from a parent object. |
| [ExternalConnection(ExternalConnection_Impl* impl)](../externalconnection/externalconnection/) | Constructs from an implementation object. |
| [ExternalConnection(const ExternalConnection\& src)](../externalconnection/externalconnection/) | Copy constructor. |
| [GetBackgroundRefresh()](../externalconnection/getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| virtual [GetClassType()](./getclasstype/) | Gets the type of this [ExternalConnection](../externalconnection/) object. |
| [GetCommand()](./getcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [GetCommandType()](./getcommandtype/) | Specifies the OLE DB command type. |
| [GetConnectionDescription()](../externalconnection/getconnectiondescription/) | Specifies the user description for this connection. |
| [GetConnectionFile()](../externalconnection/getconnectionfile/) | Gets the connection file. |
| [GetConnectionId()](../externalconnection/getconnectionid/) |  **(Deprecated)** Specifies The unique identifier of this connection. |
| [GetConnectionInfo()](./getconnectioninfo/) |  **(Deprecated)** The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [GetConnectionString()](./getconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [GetCredentialsMethodType()](../externalconnection/getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [GetId()](../externalconnection/getid/) | Gets the id of the connection. |
| [GetKeepAlive()](../externalconnection/getkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [GetName()](../externalconnection/getname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [GetOdcFile()](../externalconnection/getodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [GetOnlyUseConnectionFile()](../externalconnection/getonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [GetParameters()](../externalconnection/getparameters/) | Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
| [GetPowerQueryFormula()](./getpowerqueryformula/) | Gets the definition of power query formula. |
| [GetReconnectionMethodType()](../externalconnection/getreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [GetRefreshInternal()](../externalconnection/getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [GetRefreshOnLoad()](../externalconnection/getrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [GetSaveData()](../externalconnection/getsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [GetSavePassword()](../externalconnection/getsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [GetSecondCommand()](./getsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [GetSeverCommand()](./getsevercommand/) |  **(Deprecated)** Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [GetSourceFile()](../externalconnection/getsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [GetSourceType()](../externalconnection/getsourcetype/) | Gets or Sets the external connection DataSource type. |
| [GetSSOId()](../externalconnection/getssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [IsDeleted()](../externalconnection/isdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [IsNew()](../externalconnection/isnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DBConnection\& src)](./operator_asm/) | operator= |
| [operator=(const ExternalConnection\& src)](../externalconnection/operator_asm/) | operator= |
| [SetBackgroundRefresh(bool value)](../externalconnection/setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [SetCommand(const U16String\& value)](./setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommand(const char16_t* value)](./setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommandType(OLEDBCommandType value)](./setcommandtype/) | Specifies the OLE DB command type. |
| [SetConnectionDescription(const U16String\& value)](../externalconnection/setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionDescription(const char16_t* value)](../externalconnection/setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionInfo(const U16String\& value)](./setconnectioninfo/) |  **(Deprecated)** The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetConnectionInfo(const char16_t* value)](./setconnectioninfo/) |  **(Deprecated)** The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetConnectionString(const U16String\& value)](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetConnectionString(const char16_t* value)](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetCredentialsMethodType(CredentialsMethodType value)](../externalconnection/setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [SetIsDeleted(bool value)](../externalconnection/setisdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [SetIsNew(bool value)](../externalconnection/setisnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [SetKeepAlive(bool value)](../externalconnection/setkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [SetName(const U16String\& value)](../externalconnection/setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetName(const char16_t* value)](../externalconnection/setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetOdcFile(const U16String\& value)](../externalconnection/setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOdcFile(const char16_t* value)](../externalconnection/setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOnlyUseConnectionFile(bool value)](../externalconnection/setonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [SetReconnectionMethodType(ReConnectionMethodType value)](../externalconnection/setreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [SetRefreshInternal(int32_t value)](../externalconnection/setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [SetRefreshOnLoad(bool value)](../externalconnection/setrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [SetSaveData(bool value)](../externalconnection/setsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [SetSavePassword(bool value)](../externalconnection/setsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SetSecondCommand(const U16String\& value)](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSecondCommand(const char16_t* value)](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSeverCommand(const U16String\& value)](./setsevercommand/) |  **(Deprecated)** Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSeverCommand(const char16_t* value)](./setsevercommand/) |  **(Deprecated)** Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSourceFile(const U16String\& value)](../externalconnection/setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceFile(const char16_t* value)](../externalconnection/setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceType(ConnectionDataSourceType value)](../externalconnection/setsourcetype/) | Gets or Sets the external connection DataSource type. |
| [SetSSOId(const U16String\& value)](../externalconnection/setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [SetSSOId(const char16_t* value)](../externalconnection/setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [~DBConnection()](./~dbconnection/) | Destructor. |
| [~ExternalConnection()](../externalconnection/~externalconnection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [ExternalConnection](../externalconnection/)
* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
