##WebQueryConnection Class
'WebQueryConnection class. Encapsulates the object that represents webqueryconnection in Go.'
## WebQueryConnection class
Specifies the properties for a web query source. A web query will retrieve data from HTML tables,and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML byincluding the parameters and parameter elements.
```go
type WebQueryConnection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWebQueryConnection](./newwebqueryconnection/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetClassType](./getclasstype/) | Gets the type of this ExternalConnection object. |
|[IsXml](./isxml/) | true if the web query source is XML (versus HTML), otherwise false. |
|[SetIsXml](./setisxml/) | true if the web query source is XML (versus HTML), otherwise false. |
|[IsXl97](./isxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is setto true if this web query was created in Microsoft Excel 97.This is an optional attribute that can be ignored. |
|[SetIsXl97](./setisxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is setto true if this web query was created in Microsoft Excel 97.This is an optional attribute that can be ignored. |
|[IsXl2000](./isxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is setto true if this web query was refreshed in a spreadsheet application newer than or equalto Microsoft Excel 2000.This is an optional attribute that can be ignored. |
|[SetIsXl2000](./setisxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is setto true if this web query was refreshed in a spreadsheet application newer than or equalto Microsoft Excel 2000.This is an optional attribute that can be ignored. |
|[GetUrl](./geturl/) | URL to use to refresh external data. |
|[SetUrl](./seturl/) | URL to use to refresh external data. |
|[GetConnectionFile](./getconnectionfile/) | Gets the connection file. |
|[IsTextDates](./istextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
|[SetIsTextDates](./setistextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
|[IsXmlSourceData](./isxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
|[SetIsXmlSourceData](./setisxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
|[GetPost](./getpost/) | Returns or sets the string used with the post method of inputting data into a web serverto return data from a web query. |
|[SetPost](./setpost/) | Returns or sets the string used with the post method of inputting data into a web serverto return data from a web query. |
|[IsParsePre](./isparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page isparsed into columns when you import the page into a query table. |
|[SetIsParsePre](./setisparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page isparsed into columns when you import the page into a query table. |
|[IsHtmlTables](./ishtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
|[SetIsHtmlTables](./setishtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
|[GetHtmlFormat](./gethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into theworksheet. Relevant when sourceData is True. |
|[SetHtmlFormat](./sethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into theworksheet. Relevant when sourceData is True. |
|[IsSameSettings](./issamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settingsas the first row. |
|[SetIsSameSettings](./setissamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settingsas the first row. |
|[GetEditWebPage](./geteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persistedin the case that sourceData="true" and url has been redirected to reference an XML file.Then the user-facing page can be shown in the UI, and the XML data can be retrievedbehind the scenes. |
|[SetEditWebPage](./seteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persistedin the case that sourceData="true" and url has been redirected to reference an XML file.Then the user-facing page can be shown in the UI, and the XML data can be retrievedbehind the scenes. |
|[IsConsecutive](./isconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
|[SetIsConsecutive](./setisconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
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
|[GetPowerQueryFormula](./getpowerqueryformula/) | Gets the definition of power query formula. |
|[GetCommand](./getcommand/) | The string containing the database command to pass to the data provider API that willinteract with the external source in order to retrieve data |
|[SetCommand](./setcommand/) | The string containing the database command to pass to the data provider API that willinteract with the external source in order to retrieve data |
|[GetCommandType](./getcommandtype/) | Specifies the OLE DB command type.1. Query specifies a cube name2. Query specifies a SQL statement3. Query specifies a table name4. Query specifies that default information has been given, and it is up to the provider how to interpret.5. Query is against a web based List Data Provider. |
|[SetCommandType](./setcommandtype/) | Specifies the OLE DB command type.1. Query specifies a cube name2. Query specifies a SQL statement3. Query specifies a table name4. Query specifies that default information has been given, and it is up to the provider how to interpret.5. Query is against a web based List Data Provider. |
|[GetConnectionString](./getconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
|[SetConnectionString](./setconnectionstring/) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
|[GetSecondCommand](./getsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed |
|[SetSecondCommand](./setsecondcommand/) | Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed |
