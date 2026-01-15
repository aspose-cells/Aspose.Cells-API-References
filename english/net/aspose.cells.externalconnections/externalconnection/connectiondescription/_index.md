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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Add a worksheet with sample data
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // Create a pivot table to establish an external connection
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Get the external connection from the pivot table
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Display the initial ConnectionDescription value
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // Set a new description (since it's read-write)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // Clear the description
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // Save the workbook with the modified connection
                workbook.Save("ConnectionDescriptionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


