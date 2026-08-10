---
title: "WebQueryConnection Class"
linktitle: "WebQueryConnection"
articleTitle: "WebQueryConnection"
second_title: "Aspose.Cells for Python via Java"
description: "Specifies the properties for a web query source."
type: docs
weight: 7520
url: /python-java/asposecells.api/webqueryconnection/
---

## WebQueryConnection class

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ClassType](#classtype) | int | The value of the property is ExternalConnectionClassType integer constant. |
| [IsXml](#isxml) | boolean | true if the web query source is XML (versus HTML), otherwise false. |
| [IsXl97](#isxl97) | boolean | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [IsXl2000](#isxl2000) | boolean | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query  |
| [Url](#url) | String | URL to use to refresh external data. |
| [ConnectionFile](#connectionfile) | String |  |
| [IsTextDates](#istextdates) | boolean | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [IsXmlSourceData](#isxmlsourcedata) | boolean | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [Post](#post) | String | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query |
| [IsParsePre](#isparsepre) | boolean | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the p |
| [IsHtmlTables](#ishtmltables) | boolean | Flag indicating whether web queries should only work on HTML tables. |
| [HtmlFormat](#htmlformat) | int | How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData  |
| [IsSameSettings](#issamesettings) | boolean | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [EditWebPage](#editwebpage) | String | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [EditPage](#editpage) | String | The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" |
| [IsConsecutive](#isconsecutive) | boolean | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [Id](#id) | int | Gets the id of the connection. |
| [ConnectionId](#connectionid) | int | Specifies The unique identifier of this connection. |
| [PowerQueryFormula](#powerqueryformula) | PowerQueryFormula | Gets the definition of power query formula. |
| [Type](#type) | ConnectionDataSourceType | Gets or Sets the external connection DataSource type. |
| [SourceType](#sourcetype) | ConnectionDataSourceType |  |
| [SSOId](#ssoid) | String | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [SavePassword](#savepassword) | boolean | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SaveData](#savedata) | boolean | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [RefreshOnLoad](#refreshonload) | boolean | True if this connection should be refreshed when opening the file; otherwise, false. |
| [ReconnectionMethodType](#reconnectionmethodtype) | int | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [ReconnectionMethod](#reconnectionmethod) | int | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [OnlyUseConnectionFile](#onlyuseconnectionfile) | boolean | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [OdcFile](#odcfile) | String | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [SourceFile](#sourcefile) | String | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |
| [IsNew](#isnew) | boolean | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [Name](#name) | String | Specifies the name of the connection. Each connection must have a unique name. |
| [KeepAlive](#keepalive) | boolean | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [RefreshInternal](#refreshinternal) | int | Specifies the number of minutes between automatic refreshes of the connection. |
| [ConnectionDescription](#connectiondescription) | String | Specifies the user description for this connection |
| [IsDeleted](#isdeleted) | boolean | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [CredentialsMethodType](#credentialsmethodtype) | int | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [Credentials](#credentials) | int | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [BackgroundRefresh](#backgroundrefresh) | boolean | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [Parameters](#parameters) | ConnectionParameterCollection | Gets ConnectionParameterCollection for an ODBC or web query. |
| [Command](#command) | String |  |
| [CommandType](#commandtype) | int | The value of the property is OLEDBCommandType integer constant. |
| [ConnectionString](#connectionstring) | String |  |
| [SecondCommand](#secondcommand) | String |  |

### WebQueryConnection.ClassType property {#classtype}

The value of the property is ExternalConnectionClassType integer constant.

**Type:** int

### WebQueryConnection.IsXml property {#isxml}

true if the web query source is XML (versus HTML), otherwise false.

**Type:** boolean

### WebQueryConnection.IsXl97 property {#isxl97}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored.

**Type:** boolean

### WebQueryConnection.IsXl2000 property {#isxl2000}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored.

**Type:** boolean

### WebQueryConnection.Url property {#url}

URL to use to refresh external data.

**Type:** String

### WebQueryConnection.ConnectionFile property {#connectionfile}

**Type:** String

### WebQueryConnection.IsTextDates property {#istextdates}

Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates.

**Type:** boolean

### WebQueryConnection.IsXmlSourceData property {#isxmlsourcedata}

Flag indicating that XML source data should be imported instead of the HTML table itself.

**Type:** boolean

### WebQueryConnection.Post property {#post}

Returns or sets the string used with the post method of inputting data into a web server to return data from a web query.

**Type:** String

### WebQueryConnection.IsParsePre property {#isparsepre}

Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table.

**Type:** boolean

### WebQueryConnection.IsHtmlTables property {#ishtmltables}

Flag indicating whether web queries should only work on HTML tables.

**Type:** boolean

### WebQueryConnection.HtmlFormat property {#htmlformat}

How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. The value of the property is HtmlFormatHandlingType integer constant.

**Type:** int

### WebQueryConnection.IsSameSettings property {#issamesettings}

Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row.

**Type:** boolean

### WebQueryConnection.EditWebPage property {#editwebpage}

The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.

**Type:** String

### WebQueryConnection.EditPage property {#editpage}

The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. NOTE: This property is now obsolete. Instead, please use WebQueryConnection.EditWebPage property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** String

### WebQueryConnection.IsConsecutive property {#isconsecutive}

Flag indicating whether consecutive delimiters should be treated as just one delimiter.

**Type:** boolean

### WebQueryConnection.Id property {#id}

Gets the id of the connection.

**Type:** int

### WebQueryConnection.ConnectionId property {#connectionid}

Specifies The unique identifier of this connection.

**Type:** int

### WebQueryConnection.PowerQueryFormula property {#powerqueryformula}

Gets the definition of power query formula.

**Type:** PowerQueryFormula

### WebQueryConnection.Type property {#type}

Gets or Sets the external connection DataSource type.

**Type:** ConnectionDataSourceType

### WebQueryConnection.SourceType property {#sourcetype}

**Type:** ConnectionDataSourceType

### WebQueryConnection.SSOId property {#ssoid}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

**Type:** String

### WebQueryConnection.SavePassword property {#savepassword}

True if the password is to be saved as part of the connection string; otherwise, False.

**Type:** boolean

### WebQueryConnection.SaveData property {#savedata}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

**Type:** boolean

### WebQueryConnection.RefreshOnLoad property {#refreshonload}

True if this connection should be refreshed when opening the file; otherwise, false.

**Type:** boolean

### WebQueryConnection.ReconnectionMethodType property {#reconnectionmethodtype}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant.

**Type:** int

### WebQueryConnection.ReconnectionMethod property {#reconnectionmethod}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### WebQueryConnection.OnlyUseConnectionFile property {#onlyuseconnectionfile}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

**Type:** boolean

### WebQueryConnection.OdcFile property {#odcfile}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

**Type:** String

### WebQueryConnection.SourceFile property {#sourcefile}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

**Type:** String

### WebQueryConnection.IsNew property {#isnew}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

**Type:** boolean

### WebQueryConnection.Name property {#name}

Specifies the name of the connection. Each connection must have a unique name.

**Type:** String

### WebQueryConnection.KeepAlive property {#keepalive}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

**Type:** boolean

### WebQueryConnection.RefreshInternal property {#refreshinternal}

Specifies the number of minutes between automatic refreshes of the connection.

**Type:** int

### WebQueryConnection.ConnectionDescription property {#connectiondescription}

Specifies the user description for this connection

**Type:** String

### WebQueryConnection.IsDeleted property {#isdeleted}

Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

**Type:** boolean

### WebQueryConnection.CredentialsMethodType property {#credentialsmethodtype}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant.

**Type:** int

### WebQueryConnection.Credentials property {#credentials}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### WebQueryConnection.BackgroundRefresh property {#backgroundrefresh}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

**Type:** boolean

### WebQueryConnection.Parameters property {#parameters}

Gets ConnectionParameterCollection for an ODBC or web query.

**Type:** ConnectionParameterCollection

### WebQueryConnection.Command property {#command}

**Type:** String

### WebQueryConnection.CommandType property {#commandtype}

The value of the property is OLEDBCommandType integer constant.

**Type:** int

### WebQueryConnection.ConnectionString property {#connectionstring}

**Type:** String

### WebQueryConnection.SecondCommand property {#secondcommand}

**Type:** String
