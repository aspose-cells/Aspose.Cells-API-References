---
title: WebQueryConnection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 70
url: /python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---

## WebQueryConnection class

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, 
and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by 
including the parameters and parameter elements.



**Inheritance:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/python-net/aspose.cells.externalconnections/externalconnection)



The WebQueryConnection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [id](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Gets the id of the connection. |
| [power_query_formula](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Gets the definition of power query formula. |
| [type](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Gets or Sets the external connection DataSource type. |
| [source_file](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Used when the external data source is file-based. When a connection to such a data <br/>source fails, the spreadsheet application attempts to connect directly to this file. May be <br/>expressed in URI or system-specific file path notation. |
| [sso_id](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Identifier for Single Sign On (SSO) used for authentication between an intermediate <br/>spreadsheetML server and the external data source. |
| [save_password](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [save_data](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | True if the external data fetched over the connection to populate a table is to be saved<br/>with the workbook; otherwise, false. |
| [refresh_on_load](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [reconnection_method_type](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Specifies what the spreadsheet application should do when a connection fails.<br/>The default value is ReConnectionMethodType.Required. |
| [reconnection_method](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Specifies what the spreadsheet application should do when a connection fails.<br/>The default value is ReConnectionMethodType.Required. |
| [only_use_connection_file](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Indicates whether the spreadsheet application should always and only use the <br/>connection information in the external connection file indicated by the odcFile attribute <br/>when the connection is refreshed.  If false, then the spreadsheet application <br/>should follow the procedure indicated by the reconnectionMethod attribute |
| [odc_file](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Specifies the full path to external connection file from which this connection was <br/>created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, <br/>then the spreadsheet application will try again using information from the external connection file <br/>instead of the connection object embedded within the workbook. |
| [is_new](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | True if the connection has not been refreshed for the first time; otherwise, false. <br/>This state can happen when the user saves the file before a query has finished returning. |
| [name](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Specifies the name of the connection. Each connection must have a unique name. |
| [keep_alive](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | True when the spreadsheet application should make efforts to keep the connection <br/>open. When false, the application should close the connection after retrieving the <br/>information. |
| [refresh_internal](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Specifies the number of minutes between automatic refreshes of the connection. |
| [connection_id](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Specifies The unique identifier of this connection. |
| [connection_description](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Specifies the user description for this connection |
| [is_deleted](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) | Indicates whether the associated workbook connection has been deleted.  true if the<br/>connection has been deleted; otherwise, false. |
| [credentials_method_type](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [credentials](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [background_refresh](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Indicates whether the connection can be refreshed in the background (asynchronously). <br/>true if preferred usage of the connection is to refresh asynchronously in the background; <br/>false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [parameters](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Gets [ConnectionParameterCollection](/cells/python-net/aspose.cells.externalconnections/connectionparametercollection) for an ODBC or web query. |
| [is_xml](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | true if the web query source is XML (versus HTML), otherwise false. |
| [is_xl97](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) | This flag exists for backward compatibility with older existing spreadsheet files, and is set<br/>to true if this web query was created in Microsoft Excel 97.<br/>This is an optional attribute that can be ignored. |
| [is_xl2000](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) | This flag exists for backward compatibility with older existing spreadsheet files, and is set<br/>to true if this web query was refreshed in a spreadsheet application newer than or equal<br/>to Microsoft Excel 2000.<br/>This is an optional attribute that can be ignored. |
| [url](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL to use to refresh external data. |
| [is_text_dates](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [is_xml_source_data](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [post](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Returns or sets the string used with the post method of inputting data into a web server<br/>to return data from a web query. |
| [is_parse_pre](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) | Flag indicating whether data contained within HTML PRE tags in the web page is<br/>parsed into columns when you import the page into a query table. |
| [is_html_tables](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Flag indicating whether web queries should only work on HTML tables. |
| [html_format](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | How to handle formatting from the HTML source when bringing web query data into the<br/>worksheet. Relevant when sourceData is True. |
| [is_same_settings](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) | Flag indicating whether to parse all tables inside a PRE block with the same width settings<br/>as the first row. |
| [edit_web_page](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | The URL of the user-facing web page showing the web query data. This URL is persisted<br/>in the case that sourceData="true" and url has been redirected to reference an XML file.<br/>Then the user-facing page can be shown in the UI, and the XML data can be retrieved<br/>behind the scenes. |
| [edit_page](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | The URL of the user-facing web page showing the web query data. This URL is persisted<br/>in the case that sourceData="true" and url has been redirected to reference an XML file.<br/>Then the user-facing page can be shown in the UI, and the XML data can be retrieved<br/>behind the scenes. |
| [is_consecutive](/cells/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |



### See Also
* module [aspose.cells.externalconnections](..)
* class [ConnectionParameterCollection](/cells/python-net/aspose.cells.externalconnections/connectionparametercollection)
* class [ExternalConnection](/cells/python-net/aspose.cells.externalconnections/externalconnection)
* class [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection)
