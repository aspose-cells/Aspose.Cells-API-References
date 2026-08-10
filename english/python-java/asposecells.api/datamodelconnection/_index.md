---
title: "DataModelConnection Class"
linktitle: "DataModelConnection"
articleTitle: "DataModelConnection"
second_title: "Aspose.Cells for Python via Java"
description: "Specifies a data model connection"
type: docs
weight: 1600
url: /python-java/asposecells.api/datamodelconnection/
---

## DataModelConnection class

Specifies a data model connection

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ClassType](#classtype) | int | The value of the property is ExternalConnectionClassType integer constant. |
| [Command](#command) | String |  |
| [CommandType](#commandtype) | int | The value of the property is OLEDBCommandType integer constant. |
| [ConnectionString](#connectionstring) | String |  |
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
| [ConnectionFile](#connectionfile) | String |  |
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
| [SecondCommand](#secondcommand) | String |  |

### DataModelConnection.ClassType property {#classtype}

The value of the property is ExternalConnectionClassType integer constant.

**Type:** int

### DataModelConnection.Command property {#command}

**Type:** String

### DataModelConnection.CommandType property {#commandtype}

The value of the property is OLEDBCommandType integer constant.

**Type:** int

### DataModelConnection.ConnectionString property {#connectionstring}

**Type:** String

### DataModelConnection.Id property {#id}

Gets the id of the connection.

**Type:** int

### DataModelConnection.ConnectionId property {#connectionid}

Specifies The unique identifier of this connection.

**Type:** int

### DataModelConnection.PowerQueryFormula property {#powerqueryformula}

Gets the definition of power query formula.

**Type:** PowerQueryFormula

### DataModelConnection.Type property {#type}

Gets or Sets the external connection DataSource type.

**Type:** ConnectionDataSourceType

### DataModelConnection.SourceType property {#sourcetype}

**Type:** ConnectionDataSourceType

### DataModelConnection.SSOId property {#ssoid}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

**Type:** String

### DataModelConnection.SavePassword property {#savepassword}

True if the password is to be saved as part of the connection string; otherwise, False.

**Type:** boolean

### DataModelConnection.SaveData property {#savedata}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

**Type:** boolean

### DataModelConnection.RefreshOnLoad property {#refreshonload}

True if this connection should be refreshed when opening the file; otherwise, false.

**Type:** boolean

### DataModelConnection.ReconnectionMethodType property {#reconnectionmethodtype}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant.

**Type:** int

### DataModelConnection.ReconnectionMethod property {#reconnectionmethod}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DataModelConnection.OnlyUseConnectionFile property {#onlyuseconnectionfile}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

**Type:** boolean

### DataModelConnection.OdcFile property {#odcfile}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

**Type:** String

### DataModelConnection.SourceFile property {#sourcefile}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

**Type:** String

### DataModelConnection.ConnectionFile property {#connectionfile}

**Type:** String

### DataModelConnection.IsNew property {#isnew}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

**Type:** boolean

### DataModelConnection.Name property {#name}

Specifies the name of the connection. Each connection must have a unique name.

**Type:** String

### DataModelConnection.KeepAlive property {#keepalive}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

**Type:** boolean

### DataModelConnection.RefreshInternal property {#refreshinternal}

Specifies the number of minutes between automatic refreshes of the connection.

**Type:** int

### DataModelConnection.ConnectionDescription property {#connectiondescription}

Specifies the user description for this connection

**Type:** String

### DataModelConnection.IsDeleted property {#isdeleted}

Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

**Type:** boolean

### DataModelConnection.CredentialsMethodType property {#credentialsmethodtype}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant.

**Type:** int

### DataModelConnection.Credentials property {#credentials}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### DataModelConnection.BackgroundRefresh property {#backgroundrefresh}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

**Type:** boolean

### DataModelConnection.Parameters property {#parameters}

Gets ConnectionParameterCollection for an ODBC or web query.

**Type:** ConnectionParameterCollection

### DataModelConnection.SecondCommand property {#secondcommand}

**Type:** String
