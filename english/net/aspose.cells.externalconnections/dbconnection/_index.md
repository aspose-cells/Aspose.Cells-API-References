---
title: Class DBConnection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.DBConnection class. Specifies all properties associated with an ODBC or OLE DB external data connection
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Specifies all properties associated with an ODBC or OLE DB external data connection.

```csharp
public class DBConnection : ExternalConnection
```

## Properties

| Name | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Gets the type of this [`ExternalConnection`](../externalconnection/) object. |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Specifies the user description for this connection(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Gets the connection file.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Specifies The unique identifier of this connection.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) The connection information string is used to make contact with an OLE DB or ODBC data source. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | The connection information string is used to make contact with an OLE DB or ODBC data source. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Specifies the authentication method to be used when establishing (or re-establishing) the connection.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Specifies the authentication method to be used when establishing (or re-establishing) the connection.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Gets the id of the connection.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Specifies the name of the connection. Each connection must have a unique name.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Gets [`ConnectionParameterCollection`](../connectionparametercollection/) for an ODBC or web query.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Gets the definition of power query formula. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Specifies the number of minutes between automatic refreshes of the connection.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True if this connection should be refreshed when opening the file; otherwise, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True if the password is to be saved as part of the connection string; otherwise, False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Gets or Sets the external connection DataSource type.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Gets or Sets the external connection DataSource type.(Inherited from [`ExternalConnection`](../externalconnection/).) |

### Examples

```csharp
// Called: DBConnection conn = (DBConnection)workbook.DataConnections[0];
public void ExternalConnections_Type_DBConnection()
{
    string filePath = Constants.PivotTableSourcePath + @"NET51180_";
    string savePath = CreateFolder(filePath);

    Workbook workbook = new Workbook(filePath + "PivotTables_SourceFile.xls");

    DBConnection conn = (DBConnection)workbook.DataConnections[0];
    string command = conn.Command;
    string connectionInfo = conn.ConnectionInfo;
    Assert.Greater(command.Length, 5);
    Assert.Greater(connectionInfo.Length, 20);

    workbook.Save(savePath + "example.xlsm", Aspose.Cells.SaveFormat.Xlsm);

    string cacheXml = GetEntryText(savePath + "example.xlsm", @"xl/pivotCache/pivotCacheDefinition1.xml");
    Assert.AreNotEqual(cacheXml.IndexOf("type=\"external\""), -1);

    Workbook wb = new Workbook(savePath + "example.xlsm");
    conn = (DBConnection)wb.DataConnections[0];
    Assert.AreEqual(conn.Command, command);
    Assert.AreEqual(conn.ConnectionInfo, connectionInfo);
}
```

### See Also

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


