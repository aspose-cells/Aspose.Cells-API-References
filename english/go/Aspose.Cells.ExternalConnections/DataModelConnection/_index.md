---
title: DataModelConnection Class 
linktitle: DataModelConnection
second_title: Aspose.Cells for Go API Reference
description: 'DataModelConnection class. Encapsulates the object that represents datamodelconnection in Go.'
type: docs
weight: 200
url: /go/aspose.cells.externalconnections/datamodelconnection/
---

## DataModelConnection class

Specifies a data model connection

```go

type DataModelConnection struct 

datamodelconnection, _ := asposecells.NewDataModelConnection()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetId](./getid/) | Gets the id of the connection. | 
|[GetType](./gettype/) | Gets or Sets the external connection DataSource type. | 
|[SetType](./settype/) | Gets or Sets the external connection DataSource type. | 
|[GetSourceFile](./getsourcefile/) | Used when the external data source is file-based. When a connection to such a datasource fails, the spreadsheet application attempts to connect directly to this file. May beexpressed in URI or system-specific file path notation. | 
|[SetSourceFile](./setsourcefile/) | Used when the external data source is file-based. When a connection to such a datasource fails, the spreadsheet application attempts to connect directly to this file. May beexpressed in URI or system-specific file path notation. | 
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
|[IsNew](./isnew/) | True if the connection has not been refreshed for the first time; otherwise, false.This state can happen when the user saves the file before a query has finished returning. | 
|[SetIsNew](./setisnew/) | True if the connection has not been refreshed for the first time; otherwise, false.This state can happen when the user saves the file before a query has finished returning. | 
|[GetName](./getname/) | Specifies the name of the connection. Each connection must have a unique name. | 
|[SetName](./setname/) | Specifies the name of the connection. Each connection must have a unique name. | 
|[GetKeepAlive](./getkeepalive/) | True when the spreadsheet application should make efforts to keep the connectionopen. When false, the application should close the connection after retrieving theinformation. | 
|[SetKeepAlive](./setkeepalive/) | True when the spreadsheet application should make efforts to keep the connectionopen. When false, the application should close the connection after retrieving theinformation. | 
|[GetRefreshInternal](./getrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. | 
|[SetRefreshInternal](./setrefreshinternal/) | Specifies the number of minutes between automatic refreshes of the connection. | 
|[GetConnectionId](./getconnectionid/) | Specifies The unique identifier of this connection. | 
|[GetConnectionDescription](./getconnectiondescription/) | Specifies the user description for this connection | 
|[SetConnectionDescription](./setconnectiondescription/) | Specifies the user description for this connection | 
|[IsDeleted](./isdeleted/) | Indicates whether the associated workbook connection has been deleted.  true if theconnection has been deleted; otherwise, false. | 
|[SetIsDeleted](./setisdeleted/) | Indicates whether the associated workbook connection has been deleted.  true if theconnection has been deleted; otherwise, false. | 
|[GetCredentialsMethodType](./getcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. | 
|[SetCredentialsMethodType](./setcredentialsmethodtype/) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. | 
|[GetBackgroundRefresh](./getbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously).true if preferred usage of the connection is to refresh asynchronously in the background;false if preferred usage of the connection is to refresh synchronously in the foreground. | 
|[SetBackgroundRefresh](./setbackgroundrefresh/) | Indicates whether the connection can be refreshed in the background (asynchronously).true if preferred usage of the connection is to refresh asynchronously in the background;false if preferred usage of the connection is to refresh synchronously in the foreground. | 
|[GetParameters](./getparameters/) | Gets <see cref="ConnectionParameterCollection"/> for an ODBC or web query. | 
|[GetPowerQueryFormula](./getpowerqueryformula/) | Gets the definition of power query formula. | 
