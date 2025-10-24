##Aspose::Cells::ExternalConnections::WebQueryConnection class
'Aspose::Cells::ExternalConnections::WebQueryConnection class. Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements in C++.'
## WebQueryConnection class
Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.
```cpp
class WebQueryConnection : public Aspose::Cells::ExternalConnections::ExternalConnection
```
## Methods
| Method | Description |
| --- | --- |
| [ExternalConnection(ExternalConnection_Impl* impl)](../externalconnection/externalconnection/) | Constructs from an implementation object. |
| [ExternalConnection(const ExternalConnection\& src)](../externalconnection/externalconnection/) | Copy constructor. |
| [GetBackgroundRefresh()](../externalconnection/getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| virtual [GetClassType()](./getclasstype/) | Gets the type of this [ExternalConnection](../externalconnection/) object. |
| [GetCommand()](../externalconnection/getcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [GetCommandType()](../externalconnection/getcommandtype/) | Specifies the OLE DB command type. |
| [GetConnectionDescription()](../externalconnection/getconnectiondescription/) | Specifies the user description for this connection. |
| [GetConnectionFile()](./getconnectionfile/) | Gets the connection file. |
| [GetConnectionId()](../externalconnection/getconnectionid/) |  **(Deprecated)** Specifies The unique identifier of this connection. |
| [GetConnectionString()](../externalconnection/getconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [GetCredentialsMethodType()](../externalconnection/getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [GetEditWebPage()](./geteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [GetHtmlFormat()](./gethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. |
| [GetId()](../externalconnection/getid/) | Gets the id of the connection. |
| [GetKeepAlive()](../externalconnection/getkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [GetName()](../externalconnection/getname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [GetOdcFile()](../externalconnection/getodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [GetOnlyUseConnectionFile()](../externalconnection/getonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [GetParameters()](../externalconnection/getparameters/) | Gets [ConnectionParameterCollection](../connectionparametercollection/) for an ODBC or web query. |
| [GetPost()](./getpost/) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [GetPowerQueryFormula()](../externalconnection/getpowerqueryformula/) | Gets the definition of power query formula. |
| [GetReconnectionMethodType()](../externalconnection/getreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [GetRefreshInternal()](../externalconnection/getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [GetRefreshOnLoad()](../externalconnection/getrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [GetSaveData()](../externalconnection/getsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [GetSavePassword()](../externalconnection/getsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [GetSecondCommand()](../externalconnection/getsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [GetSourceFile()](../externalconnection/getsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [GetSourceType()](../externalconnection/getsourcetype/) | Gets or Sets the external connection DataSource type. |
| [GetSSOId()](../externalconnection/getssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [GetUrl()](./geturl/) | URL to use to refresh external data. |
| [IsConsecutive()](./isconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [IsDeleted()](../externalconnection/isdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [IsHtmlTables()](./ishtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
| [IsNew()](../externalconnection/isnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsParsePre()](./isparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [IsSameSettings()](./issamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [IsTextDates()](./istextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [IsXl2000()](./isxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored. |
| [IsXl97()](./isxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored. |
| [IsXml()](./isxml/) | true if the web query source is XML (versus HTML), otherwise false. |
| [IsXmlSourceData()](./isxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WebQueryConnection\& src)](./operator_asm/) | operator= |
| [operator=(const ExternalConnection\& src)](../externalconnection/operator_asm/) | operator= |
| [SetBackgroundRefresh(bool value)](../externalconnection/setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [SetCommand(const U16String\& value)](../externalconnection/setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommand(const char16_t* value)](../externalconnection/setcommand/) | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data. |
| [SetCommandType(OLEDBCommandType value)](../externalconnection/setcommandtype/) | Specifies the OLE DB command type. |
| [SetConnectionDescription(const U16String\& value)](../externalconnection/setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionDescription(const char16_t* value)](../externalconnection/setconnectiondescription/) | Specifies the user description for this connection. |
| [SetConnectionString(const U16String\& value)](../externalconnection/setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetConnectionString(const char16_t* value)](../externalconnection/setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [SetCredentialsMethodType(CredentialsMethodType value)](../externalconnection/setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [SetEditWebPage(const U16String\& value)](./seteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [SetEditWebPage(const char16_t* value)](./seteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [SetHtmlFormat(HtmlFormatHandlingType value)](./sethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. |
| [SetIsConsecutive(bool value)](./setisconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [SetIsDeleted(bool value)](../externalconnection/setisdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [SetIsHtmlTables(bool value)](./setishtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
| [SetIsNew(bool value)](../externalconnection/setisnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [SetIsParsePre(bool value)](./setisparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [SetIsSameSettings(bool value)](./setissamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [SetIsTextDates(bool value)](./setistextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [SetIsXl2000(bool value)](./setisxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored. |
| [SetIsXl97(bool value)](./setisxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored. |
| [SetIsXml(bool value)](./setisxml/) | true if the web query source is XML (versus HTML), otherwise false. |
| [SetIsXmlSourceData(bool value)](./setisxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [SetKeepAlive(bool value)](../externalconnection/setkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [SetName(const U16String\& value)](../externalconnection/setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetName(const char16_t* value)](../externalconnection/setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [SetOdcFile(const U16String\& value)](../externalconnection/setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOdcFile(const char16_t* value)](../externalconnection/setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [SetOnlyUseConnectionFile(bool value)](../externalconnection/setonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute. |
| [SetPost(const U16String\& value)](./setpost/) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [SetPost(const char16_t* value)](./setpost/) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [SetReconnectionMethodType(ReConnectionMethodType value)](../externalconnection/setreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is [ReConnectionMethodType.Required](../reconnectionmethodtype/). |
| [SetRefreshInternal(int32_t value)](../externalconnection/setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [SetRefreshOnLoad(bool value)](../externalconnection/setrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [SetSaveData(bool value)](../externalconnection/setsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [SetSavePassword(bool value)](../externalconnection/setsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SetSecondCommand(const U16String\& value)](../externalconnection/setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSecondCommand(const char16_t* value)](../externalconnection/setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed. |
| [SetSourceFile(const U16String\& value)](../externalconnection/setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceFile(const char16_t* value)](../externalconnection/setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SetSourceType(ConnectionDataSourceType value)](../externalconnection/setsourcetype/) | Gets or Sets the external connection DataSource type. |
| [SetSSOId(const U16String\& value)](../externalconnection/setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [SetSSOId(const char16_t* value)](../externalconnection/setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [SetUrl(const U16String\& value)](./seturl/) | URL to use to refresh external data. |
| [SetUrl(const char16_t* value)](./seturl/) | URL to use to refresh external data. |
| [WebQueryConnection(WebQueryConnection_Impl* impl)](./webqueryconnection/) | Constructs from an implementation object. |
| [WebQueryConnection(const WebQueryConnection\& src)](./webqueryconnection/) | Copy constructor. |
| [WebQueryConnection(const ExternalConnection\& src)](./webqueryconnection/) | Constructs from a parent object. |
| [~ExternalConnection()](../externalconnection/~externalconnection/) | Destructor. |
| [~WebQueryConnection()](./~webqueryconnection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [ExternalConnection](../externalconnection/)
* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
