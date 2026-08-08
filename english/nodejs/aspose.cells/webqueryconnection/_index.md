---
title: "WebQueryConnection"
linktitle: "WebQueryConnection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies the properties for a web query source."
type: docs
weight: 4660
url: /nodejs/aspose.cells/webqueryconnection/
---

## WebQueryConnection class

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.

## Methods

| Name | Description |
| --- | --- |
| [getBackgroundRefresh()](./getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [getClassType()](./getclasstype/) | The value of the property is ExternalConnectionClassType integer constant. |
| [getCommand()](./getcommand/) |  |
| [getCommandType()](./getcommandtype/) | The value of the property is OLEDBCommandType integer constant. |
| [getConnectionDescription()](./getconnectiondescription/) | Specifies the user description for this connection |
| [getConnectionFile()](./getconnectionfile/) |  |
| [getConnectionId()](./getconnectionid/) | Specifies The unique identifier of this connection. |
| [getConnectionString()](./getconnectionstring/) |  |
| [getCredentials()](./getcredentials/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [getCredentialsMethodType()](./getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [getEditPage()](./geteditpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [getEditWebPage()](./geteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [getHtmlFormat()](./gethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData  |
| [getId()](./getid/) | Gets the id of the connection. |
| [getKeepAlive()](./getkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [getName()](./getname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [getOdcFile()](./getodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [getOnlyUseConnectionFile()](./getonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [getParameters()](./getparameters/) | Gets ConnectionParameterCollection for an ODBC or web query. |
| [getPost()](./getpost/) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query |
| [getPowerQueryFormula()](./getpowerqueryformula/) | Gets the definition of power query formula. |
| [getReconnectionMethod()](./getreconnectionmethod/) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [getReconnectionMethodType()](./getreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [getRefreshInternal()](./getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [getRefreshOnLoad()](./getrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [getSSOId()](./getssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [getSaveData()](./getsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [getSavePassword()](./getsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSecondCommand()](./getsecondcommand/) |  |
| [getSourceFile()](./getsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |
| [getSourceType()](./getsourcetype/) |  |
| [getType()](./gettype/) | Gets or Sets the external connection DataSource type. |
| [getUrl()](./geturl/) | URL to use to refresh external data. |
| [isConsecutive()](./isconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [isDeleted()](./isdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [isHtmlTables()](./ishtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
| [isNew()](./isnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [isParsePre()](./isparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the p |
| [isSameSettings()](./issamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [isTextDates()](./istextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [isXl2000()](./isxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [isXl97()](./isxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [isXml()](./isxml/) | true if the web query source is XML (versus HTML), otherwise false. |
| [isXmlSourceData()](./isxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [setBackgroundRefresh()](./setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [setCommand()](./setcommand/) |  |
| [setCommandType()](./setcommandtype/) | The value of the property is OLEDBCommandType integer constant. |
| [setConnectionDescription()](./setconnectiondescription/) | Specifies the user description for this connection |
| [setConnectionString()](./setconnectionstring/) |  |
| [setConsecutive()](./setconsecutive/) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [setCredentials()](./setcredentials/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [setCredentialsMethodType()](./setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [setDeleted()](./setdeleted/) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [setEditPage()](./seteditpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [setEditWebPage()](./seteditwebpage/) | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [setHtmlFormat()](./sethtmlformat/) | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData  |
| [setHtmlTables()](./sethtmltables/) | Flag indicating whether web queries should only work on HTML tables. |
| [setKeepAlive()](./setkeepalive/) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [setName()](./setname/) | Specifies the name of the connection. Each connection must have a unique name. |
| [setNew()](./setnew/) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [setOdcFile()](./setodcfile/) | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [setOnlyUseConnectionFile()](./setonlyuseconnectionfile/) | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [setParsePre()](./setparsepre/) | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the p |
| [setPost()](./setpost/) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query |
| [setReconnectionMethod()](./setreconnectionmethod/) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [setReconnectionMethodType()](./setreconnectionmethodtype/) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [setRefreshInternal()](./setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. |
| [setRefreshOnLoad()](./setrefreshonload/) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [setSSOId()](./setssoid/) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [setSameSettings()](./setsamesettings/) | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [setSaveData()](./setsavedata/) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [setSavePassword()](./setsavepassword/) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [setSecondCommand()](./setsecondcommand/) |  |
| [setSourceFile()](./setsourcefile/) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |
| [setTextDates()](./settextdates/) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [setUrl()](./seturl/) | URL to use to refresh external data. |
| [setXl2000()](./setxl2000/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [setXl97()](./setxl97/) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [setXml()](./setxml/) | true if the web query source is XML (versus HTML), otherwise false. |
| [setXmlSourceData()](./setxmlsourcedata/) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
