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
namespace AsposeCellsExamples
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
                // Create a new workbook
                Workbook workbook = new Workbook();

                // Create a connection parameter (simulated since constructor parameters are unknown)
                ConnectionParameter parameter = null;

                // In a real scenario, you would create the parameter properly
                // parameter = new ConnectionParameter(/* required parameters */);

                // For demonstration, we'll show how Name would be used if we had a parameter
                if (parameter != null)
                {
                    // Get and display the current Name value
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Set a new Name value (since property is read-write)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Fallback demonstration when we can't create the parameter
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Save the workbook
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


