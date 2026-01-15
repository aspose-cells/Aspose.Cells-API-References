---
title: DBConnection.Command
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

```csharp
public override string Command { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the collection of external connections
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Find the first DBConnection in the collection (if any)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Display the current Command value (read operation)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Demonstrate setting the Command (read-write property)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Save the workbook
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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


