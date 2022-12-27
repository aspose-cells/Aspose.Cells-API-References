---
title: DataModelConnection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.externalconnections/datamodelconnection/
is_root: false
---

## DataModelConnection class

Specifies a data model connection



**Inheritance:** [DataModelConnection](/cells/python-net/aspose.cells.externalconnections/datamodelconnection) → 
[ExternalConnection](/cells/python-net/aspose.cells.externalconnections/externalconnection)



The DataModelConnection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [id](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/id) | Gets the id of the connection. |
| [power_query_formula](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/power_query_formula) | Gets the definition of power query formula. |
| [type](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/type) | Gets or Sets the external connection DataSource type. |
| [source_file](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/source_file) | Used when the external data source is file-based. When a connection to such a data <br/>source fails, the spreadsheet application attempts to connect directly to this file. May be <br/>expressed in URI or system-specific file path notation. |
| [sso_id](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/sso_id) | Identifier for Single Sign On (SSO) used for authentication between an intermediate <br/>spreadsheetML server and the external data source. |
| [save_password](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/save_password) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [save_data](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/save_data) | True if the external data fetched over the connection to populate a table is to be saved<br/>with the workbook; otherwise, false. |
| [refresh_on_load](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/refresh_on_load) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [reconnection_method_type](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/reconnection_method_type) | Specifies what the spreadsheet application should do when a connection fails.<br/>The default value is ReConnectionMethodType.Required. |
| [reconnection_method](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/reconnection_method) | Specifies what the spreadsheet application should do when a connection fails.<br/>The default value is ReConnectionMethodType.Required. |
| [only_use_connection_file](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/only_use_connection_file) | Indicates whether the spreadsheet application should always and only use the <br/>connection information in the external connection file indicated by the odcFile attribute <br/>when the connection is refreshed.  If false, then the spreadsheet application <br/>should follow the procedure indicated by the reconnectionMethod attribute |
| [odc_file](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/odc_file) | Specifies the full path to external connection file from which this connection was <br/>created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, <br/>then the spreadsheet application will try again using information from the external connection file <br/>instead of the connection object embedded within the workbook. |
| [is_new](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/is_new) | True if the connection has not been refreshed for the first time; otherwise, false. <br/>This state can happen when the user saves the file before a query has finished returning. |
| [name](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/name) | Specifies the name of the connection. Each connection must have a unique name. |
| [keep_alive](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/keep_alive) | True when the spreadsheet application should make efforts to keep the connection <br/>open. When false, the application should close the connection after retrieving the <br/>information. |
| [refresh_internal](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/refresh_internal) | Specifies the number of minutes between automatic refreshes of the connection. |
| [connection_id](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/connection_id) | Specifies The unique identifier of this connection. |
| [connection_description](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/connection_description) | Specifies the user description for this connection |
| [is_deleted](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/is_deleted) | Indicates whether the associated workbook connection has been deleted.  true if the<br/>connection has been deleted; otherwise, false. |
| [credentials_method_type](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/credentials_method_type) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [credentials](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/credentials) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [background_refresh](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/background_refresh) | Indicates whether the connection can be refreshed in the background (asynchronously). <br/>true if preferred usage of the connection is to refresh asynchronously in the background; <br/>false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [parameters](/cells/python-net/aspose.cells.externalconnections/datamodelconnection/parameters) | Gets [ConnectionParameterCollection](/cells/python-net/aspose.cells.externalconnections/connectionparametercollection) for an ODBC or web query. |


### See Also

* module [aspose.cells.externalconnections](../)
* class [ExternalConnection](/cells/python-net/aspose.cells.externalconnections/externalconnection)
