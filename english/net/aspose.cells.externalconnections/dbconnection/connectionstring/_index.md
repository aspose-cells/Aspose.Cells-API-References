---
title: DBConnection.ConnectionString
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

The connection information string is used to make contact with an OLE DB or ODBC data source.

```csharp
public override string ConnectionString { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the collection of external connections
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Create a new DBConnection by adding it to the collection
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Display the initial ConnectionString value
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Set a new connection string
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Display the updated ConnectionString value
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Save the workbook
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


