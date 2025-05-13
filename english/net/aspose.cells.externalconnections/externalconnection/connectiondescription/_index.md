---
title: ExternalConnection.ConnectionDescription
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the user description for this connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Specifies the user description for this connection

```csharp
public string ConnectionDescription { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Description info: " + dataModelConnection.ConnectionDescription);
public void ExternalConnection_Property_ConnectionDescription()
{
    string filePath = Constants.PivotTableSourcePath + @"NET52065_";

    Workbook workbook = new Workbook(filePath + "RRI_Template_DataSQL.xlsb");
    int dbCount = 0;
    int dataModelCount = 0;
    for (int i = 0; i < workbook.DataConnections.Count; i++)
    {
        Aspose.Cells.ExternalConnections.ExternalConnection externalConnection = workbook.DataConnections[i];
        if (externalConnection is DBConnection)
        {
            DBConnection dbConn = externalConnection as DBConnection;
            Console.WriteLine("Connection Name: " + dbConn.Name);
            Console.WriteLine("Info: " + dbConn.ConnectionInfo);
            Console.WriteLine("Command type: " + dbConn.CommandType);
            Console.WriteLine("Command: " + dbConn.Command);
            Console.WriteLine("Description: " + dbConn.ConnectionDescription);
            Console.WriteLine("Id: " + dbConn.Id);
            Console.WriteLine("Credentials: " + dbConn.CredentialsMethodType);
            Console.WriteLine("Type: " + dbConn.SourceType);
            Console.WriteLine("########################");
            dbCount++;
        }
        else if (externalConnection is DataModelConnection)
        {
            DataModelConnection dataModelConnection = externalConnection as DataModelConnection;
            Console.WriteLine("Connection Name: " + dataModelConnection.Name);
            Console.WriteLine("Description info: " + dataModelConnection.ConnectionDescription);
            Console.WriteLine("Connection ID: " + dataModelConnection.Id);
            Console.WriteLine("Credentials: " + dataModelConnection.CredentialsMethodType);
            Console.WriteLine("Type: " + dataModelConnection.SourceType);
            Console.WriteLine("########################");
            dataModelCount++;

        }
        else
        {

            Console.WriteLine("Connection Name: " + workbook.DataConnections[i].Name);
            Console.WriteLine("Description info: " + workbook.DataConnections[i].ConnectionDescription);
            Console.WriteLine("Connection ID: " + workbook.DataConnections[i].Id);
            Console.WriteLine("Credentials: " + workbook.DataConnections[i].CredentialsMethodType);
            Console.WriteLine("Type: " + workbook.DataConnections[i].SourceType);
            Console.WriteLine("########################");
        }
    }

    Assert.AreEqual(dbCount, 1);
    Assert.AreEqual(dataModelCount, 3);
}
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


