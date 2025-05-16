---
title: WebQueryConnection.IsXl2000
second_title: Aspose.Cells for .NET API Reference
description: WebQueryConnection property. This flag exists for backward compatibility with older existing spreadsheet files and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored
type: docs
url: /net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored.

```csharp
public bool IsXl2000 { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.WebQueryConnectionPropertyIsXl2000Demo
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the first existing web query connection (if any)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Display initial IsXl2000 value
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Set IsXl2000 to true (since it's read-write)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Set IsXl2000 back to false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Save the workbook
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


