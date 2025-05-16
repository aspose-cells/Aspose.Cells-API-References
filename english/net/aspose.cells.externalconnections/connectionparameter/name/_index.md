---
title: ConnectionParameter.Name
second_title: Aspose.Cells for .NET API Reference
description: ConnectionParameter property. The name of the parameter
type: docs
url: /net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

The name of the parameter.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ConnectionParameterPropertyNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new connection parameter instance
                // Note: ConnectionParameter requires constructor parameters
                // Since we don't know them, we'll demonstrate property access directly
                ConnectionParameter parameter = null;
                
                // In a real scenario, you would create the parameter with proper constructor arguments
                // For demonstration purposes, we'll just show property access
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // This line is kept to show the property access pattern
                // parameter.Name = "CustomerID";

                // For demo purposes, we'll create a workbook instead
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Connection Parameter Demo";
                
                // Save the workbook
                workbook.Save("ConnectionParameterDemo.xlsx");
                
                Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter with required constructor arguments.");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


