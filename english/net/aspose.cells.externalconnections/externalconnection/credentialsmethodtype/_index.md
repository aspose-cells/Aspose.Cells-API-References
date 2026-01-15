---
title: ExternalConnection.CredentialsMethodType
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the authentication method to be used when establishing or reestablishing the connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Specifies the authentication method to be used when establishing (or re-establishing) the connection.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Add a worksheet and create a pivot table to establish an external connection
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Create pivot table which will have an external connection
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Get the external connection from the pivot table
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Display the current CredentialsMethodType value
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Demonstrate setting the property (since it's read-write)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Set to another value to demonstrate
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Save the workbook with the modified connection settings
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


