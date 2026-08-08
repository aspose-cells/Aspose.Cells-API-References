---
title: "DBConnection"
linktitle: "DBConnection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies all properties associated with an ODBC or OLE DB external data connection."
type: docs
weight: 980
url: /nodejs/aspose.cells/dbconnection/
---

## DBConnection class

Specifies all properties associated with an ODBC or OLE DB external data connection.

## Methods

| Name | Description |
| --- | --- |
| [getBackgroundRefresh()](#getbackgroundrefresh) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [getClassType()](#getclasstype) | The value of the property is ExternalConnectionClassType integer constant. |
| [getCommand()](#getcommand) | The string containing the database command to pass to the data provider API that will interact with the external source  |
| [getCommandType()](#getcommandtype) | Specifies the OLE DB command type. |
| [getConnectionDescription()](#getconnectiondescription) | Specifies the user description for this connection |
| [getConnectionFile()](#getconnectionfile) |  |
| [getConnectionId()](#getconnectionid) | Specifies The unique identifier of this connection. |
| [getConnectionInfo()](#getconnectioninfo) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [getConnectionString()](#getconnectionstring) |  |
| [getCredentials()](#getcredentials) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [getCredentialsMethodType()](#getcredentialsmethodtype) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [getId()](#getid) | Gets the id of the connection. |
| [getKeepAlive()](#getkeepalive) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [getName()](#getname) | Specifies the name of the connection. Each connection must have a unique name. |
| [getOdcFile()](#getodcfile) | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [getOnlyUseConnectionFile()](#getonlyuseconnectionfile) | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [getParameters()](#getparameters) | Gets ConnectionParameterCollection for an ODBC or web query. |
| [getPowerQueryFormula()](#getpowerqueryformula) | Gets the definition of power query formula. |
| [getReconnectionMethod()](#getreconnectionmethod) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [getReconnectionMethodType()](#getreconnectionmethodtype) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [getRefreshInternal()](#getrefreshinternal) | Specifies the number of minutes between automatic refreshes of the connection. |
| [getRefreshOnLoad()](#getrefreshonload) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [getSSOId()](#getssoid) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [getSaveData()](#getsavedata) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [getSavePassword()](#getsavepassword) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSecondCommand()](#getsecondcommand) |  |
| [getSeverCommand()](#getsevercommand) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC c |
| [getSourceFile()](#getsourcefile) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |
| [getSourceType()](#getsourcetype) |  |
| [getType()](#gettype) | Gets or Sets the external connection DataSource type. |
| [isDeleted()](#isdeleted) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [isNew()](#isnew) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [setBackgroundRefresh()](#setbackgroundrefresh) | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the con |
| [setCommand()](#setcommand) | The string containing the database command to pass to the data provider API that will interact with the external source  |
| [setCommandType()](#setcommandtype) | Specifies the OLE DB command type. |
| [setConnectionDescription()](#setconnectiondescription) | Specifies the user description for this connection |
| [setConnectionInfo()](#setconnectioninfo) | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [setConnectionString()](#setconnectionstring) |  |
| [setCredentials()](#setcredentials) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [setCredentialsMethodType()](#setcredentialsmethodtype) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the p |
| [setDeleted()](#setdeleted) | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwis |
| [setKeepAlive()](#setkeepalive) | True when the spreadsheet application should make efforts to keep the connection open. When false, the application shoul |
| [setName()](#setname) | Specifies the name of the connection. Each connection must have a unique name. |
| [setNew()](#setnew) | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user  |
| [setOdcFile()](#setodcfile) | Specifies the full path to external connection file from which this connection was created. If a connection fails during |
| [setOnlyUseConnectionFile()](#setonlyuseconnectionfile) | Indicates whether the spreadsheet application should always and only use the connection information in the external conn |
| [setReconnectionMethod()](#setreconnectionmethod) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [setReconnectionMethodType()](#setreconnectionmethodtype) | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodTyp |
| [setRefreshInternal()](#setrefreshinternal) | Specifies the number of minutes between automatic refreshes of the connection. |
| [setRefreshOnLoad()](#setrefreshonload) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [setSSOId()](#setssoid) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the externa |
| [setSaveData()](#setsavedata) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, f |
| [setSavePassword()](#setsavepassword) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [setSecondCommand()](#setsecondcommand) |  |
| [setSeverCommand()](#setsevercommand) | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC c |
| [setSourceFile()](#setsourcefile) | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet applica |

### getBackgroundRefresh() {#getbackgroundrefresh}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

### getClassType() {#getclasstype}

The value of the property is ExternalConnectionClassType integer constant.

### getCommand() {#getcommand}

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

### getCommandType() {#getcommandtype}

Specifies the OLE DB command type.

### getConnectionDescription() {#getconnectiondescription}

Specifies the user description for this connection

### getConnectionFile() {#getconnectionfile}

### getConnectionId() {#getconnectionid}

Specifies The unique identifier of this connection.

### getConnectionInfo() {#getconnectioninfo}

The connection information string is used to make contact with an OLE DB or ODBC data source.

### getConnectionString() {#getconnectionstring}

### getCredentials() {#getcredentials}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

### getCredentialsMethodType() {#getcredentialsmethodtype}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant.

### getId() {#getid}

Gets the id of the connection.

### getKeepAlive() {#getkeepalive}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

### getName() {#getname}

Specifies the name of the connection. Each connection must have a unique name.

### getOdcFile() {#getodcfile}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

### getOnlyUseConnectionFile() {#getonlyuseconnectionfile}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

### getParameters() {#getparameters}

Gets ConnectionParameterCollection for an ODBC or web query.

### getPowerQueryFormula() {#getpowerqueryformula}

Gets the definition of power query formula.

### getReconnectionMethod() {#getreconnectionmethod}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

### getReconnectionMethodType() {#getreconnectionmethodtype}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant.

### getRefreshInternal() {#getrefreshinternal}

Specifies the number of minutes between automatic refreshes of the connection.

### getRefreshOnLoad() {#getrefreshonload}

True if this connection should be refreshed when opening the file; otherwise, false.

### getSSOId() {#getssoid}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

### getSaveData() {#getsavedata}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

### getSavePassword() {#getsavepassword}

True if the password is to be saved as part of the connection string; otherwise, False.

### getSecondCommand() {#getsecondcommand}

### getSeverCommand() {#getsevercommand}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

### getSourceFile() {#getsourcefile}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

### getSourceType() {#getsourcetype}

### getType() {#gettype}

Gets or Sets the external connection DataSource type.

### isDeleted() {#isdeleted}

Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

### isNew() {#isnew}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

### setBackgroundRefresh() {#setbackgroundrefresh}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

### setCommand() {#setcommand}

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

### setCommandType() {#setcommandtype}

Specifies the OLE DB command type.

### setConnectionDescription() {#setconnectiondescription}

Specifies the user description for this connection

### setConnectionInfo() {#setconnectioninfo}

The connection information string is used to make contact with an OLE DB or ODBC data source.

### setConnectionString() {#setconnectionstring}

### setCredentials() {#setcredentials}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

### setCredentialsMethodType() {#setcredentialsmethodtype}

Specifies the authentication method to be used when establishing (or re-establishing) the connection. The value of the property is CredentialsMethodType integer constant.

### setDeleted() {#setdeleted}

Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

### setKeepAlive() {#setkeepalive}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

### setName() {#setname}

Specifies the name of the connection. Each connection must have a unique name.

### setNew() {#setnew}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

### setOdcFile() {#setodcfile}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

### setOnlyUseConnectionFile() {#setonlyuseconnectionfile}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

### setReconnectionMethod() {#setreconnectionmethod}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

### setReconnectionMethodType() {#setreconnectionmethodtype}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. The value of the property is ReConnectionMethodType integer constant.

### setRefreshInternal() {#setrefreshinternal}

Specifies the number of minutes between automatic refreshes of the connection.

### setRefreshOnLoad() {#setrefreshonload}

True if this connection should be refreshed when opening the file; otherwise, false.

### setSSOId() {#setssoid}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

### setSaveData() {#setsavedata}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

### setSavePassword() {#setsavepassword}

True if the password is to be saved as part of the connection string; otherwise, False.

### setSecondCommand() {#setsecondcommand}

### setSeverCommand() {#setsevercommand}

Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

### setSourceFile() {#setsourcefile}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.
