---
title: DBConnection.CommandType
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Initialize a workbook (empty or from a file that may contain connections)
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
                    // Display the current CommandType value
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Demonstrate setting the CommandType (read‑write property)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Save the workbook (even if unchanged) to illustrate a complete flow
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


