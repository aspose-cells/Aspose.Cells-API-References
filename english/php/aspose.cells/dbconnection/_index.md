---
title: "DBConnection Class"
linktitle: "DBConnection"
articleTitle: "DBConnection"
second_title: "Aspose.Cells for PHP via Java"
description: "Specifies all properties associated with an ODBC or OLE DB external data connection."
type: docs
weight: 1480
url: /php/aspose.cells/dbconnection/
---

## DBConnection class

Specifies all properties associated with an ODBC or OLE DB external data connection.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ClassType](#classtype) | Number | The value of the property is ExternalConnectionClassType integer constant. |
| [ConnectionString](#connectionstring) | String |  |
| [ConnectionInfo](#connectioninfo) | String | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [PowerQueryFormula](#powerqueryformula) | PowerQueryFormula | Gets the definition of power query formula. |
| [CommandType](#commandtype) | Number | Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies  |
| [Command](#command) | String | The string containing the database command to pass to the data provider API that will interact with the external source  |
| [SeverCommand](#severcommand) | String | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC c |
| [SecondCommand](#secondcommand) | String |  |
| [Id](#id) | Number | Gets the id of the connection. |
| [ConnectionId](#connectionid) | Number | Specifies The unique identifier of this connection. |
| [Type](#type) | ConnectionDataSourceType | Gets or Sets the external connection DataSource type. |
| [SourceType](#sourcetype) | ConnectionDataSourceType |  |
| [SSOId](#ssoid) | String | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [SavePassword](#savepassword) | boolean | True if the password is to be saved as part of the connection string; otherwise, False. |
| [SaveData](#savedata) | boolean | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [RefreshOnLoad](#refreshonload) | boolean | True if this connection should be refreshed when opening the file; otherwise, false. |
| [ReconnectionMethodType](#reconnectionmethodtype) | Number | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [ReconnectionMethod](#reconnectionmethod) | Number | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [OnlyUseConnectionFile](#onlyuseconnectionfile) | boolean | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [OdcFile](#odcfile) | String | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [SourceFile](#sourcefile) | String | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |
| [ConnectionFile](#connectionfile) | String |  |
| [IsNew](#isnew) | boolean | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [Name](#name) | String | Specifies the name of the connection. Each connection must have a unique name. |
| [KeepAlive](#keepalive) | boolean | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [RefreshInternal](#refreshinternal) | Number | Specifies the number of minutes between automatic refreshes of the connection. |
| [ConnectionDescription](#connectiondescription) | String | Specifies the user description for this connection |
| [IsDeleted](#isdeleted) | boolean | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [CredentialsMethodType](#credentialsmethodtype) | Number | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [Credentials](#credentials) | Number | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [BackgroundRefresh](#backgroundrefresh) | boolean | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [Parameters](#parameters) | ConnectionParameterCollection | Gets ConnectionParameterCollection for an ODBC or web query. |

### DBConnection.ClassType property {#classtype}

The value of the property is ExternalConnectionClassType integer constant.

**Type:** Number

### DBConnection.ConnectionString property {#connectionstring}

**Type:** String

### DBConnection.ConnectionInfo property {#connectioninfo}

The connection information string is used to make contact with an OLE DB or ODBC data source.

**Type:** String

### DBConnection.PowerQueryFormula property {#powerqueryformula}

Gets the definition of power query formula.

**Type:** PowerQueryFormula

### DBConnection.CommandType property {#commandtype}

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. The value of the property is OLEDBCommandType integer constant.

**Type:** Number

### DBConnection.Command property {#command}

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

**Type:** String

### DBConnection.SeverCommand property {#severcommand}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

**Type:** String

### DBConnection.SecondCommand property {#secondcommand}

**Type:** String

### DBConnection.Id property {#id}

Gets the id of the connection.

**Type:** Number

### DBConnection.ConnectionId property {#connectionid}

Specifies The unique identifier of this connection.

**Type:** Number

### DBConnection.Type property {#type}

Gets or Sets the external connection DataSource type.

**Type:** ConnectionDataSourceType

### DBConnection.SourceType property {#sourcetype}

**Type:** ConnectionDataSourceType

### DBConnection.SSOId property {#ssoid}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

**Type:** String

### DBConnection.SavePassword property {#savepassword}

True if the password is to be saved as part of the connection string; otherwise, False.

**Type:** boolean

### DBConnection.SaveData property {#savedata}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

**Type:** boolean

### DBConnection.RefreshOnLoad property {#refreshonload}

True if this connection should be refreshed when opening the file; otherwise, false.

**Type:** boolean

### DBConnection.ReconnectionMethodType property {#reconnectionmethodtype}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant.

**Type:** Number

### DBConnection.ReconnectionMethod property {#reconnectionmethod}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### DBConnection.OnlyUseConnectionFile property {#onlyuseconnectionfile}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

**Type:** boolean

### DBConnection.OdcFile property {#odcfile}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

**Type:** String

### DBConnection.SourceFile property {#sourcefile}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

**Type:** String

### DBConnection.ConnectionFile property {#connectionfile}

**Type:** String

### DBConnection.IsNew property {#isnew}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

**Type:** boolean

### DBConnection.Name property {#name}

Specifies the name of the connection. Each connection must have a unique name.

**Type:** String

### DBConnection.KeepAlive property {#keepalive}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

**Type:** boolean

### DBConnection.RefreshInternal property {#refreshinternal}

Specifies the number of minutes between automatic refreshes of the connection.

**Type:** Number

### DBConnection.ConnectionDescription property {#connectiondescription}

Specifies the user description for this connection

**Type:** String

### DBConnection.IsDeleted property {#isdeleted}

Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

**Type:** boolean

### DBConnection.CredentialsMethodType property {#credentialsmethodtype}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant.

**Type:** Number

### DBConnection.Credentials property {#credentials}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### DBConnection.BackgroundRefresh property {#backgroundrefresh}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

**Type:** boolean

### DBConnection.Parameters property {#parameters}

Gets ConnectionParameterCollection for an ODBC or web query.

**Type:** ConnectionParameterCollection
