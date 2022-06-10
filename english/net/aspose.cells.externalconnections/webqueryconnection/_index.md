---
title: WebQueryConnection
second_title: Aspose.Cells for .NET API Reference
description: Specifies the properties for a web query source. A web query will retrieve data from HTML tables and can also supply HTTP Get parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.
type: docs
weight: 3370
url: /net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Properties

| Name | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Specifies the user description for this connection |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Specifies The unique identifier of this connection. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials) { get; set; } | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage) { get; set; } | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Gets the id of the connection. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Flag indicating whether web queries should only work on HTML tables. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | true if the web query source is XML (versus HTML), otherwise false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Specifies the name of the connection. Each connection must have a unique name. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Gets [`ConnectionParameterCollection`](../connectionparametercollection) for an ODBC or web query. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Gets the definition of power query formula. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod) { get; set; } | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Specifies the number of minutes between automatic refreshes of the connection. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True if this connection should be refreshed when opening the file; otherwise, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Gets or Sets the external connection DataSource type. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | URL to use to refresh external data. |

### See Also

* class [ExternalConnection](../externalconnection)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
