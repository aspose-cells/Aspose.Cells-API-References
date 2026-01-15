---
title: Enum HtmlFormatHandlingType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.HtmlFormatHandlingType enum. Specifies how to handle formatting from the HTML source
type: docs
url: /net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

Specifies how to handle formatting from the HTML source

```csharp
public enum HtmlFormatHandlingType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| All | `0` | Transfer all HTML formatting into the worksheet along with data. |
| None | `1` | Bring data in as unformatted text (setting data types still occurs). |
| Rtf | `2` | Translate HTML formatting to rich text formatting on the data brought into the worksheet. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrate all enum values of HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Display the enum values
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Simulate using these values in a scenario
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Save the workbook
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


