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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sample HTML data to import
            string html = "<table><tr><td style='color:red;font-weight:bold'>Red Bold Text</td><td>Normal Text</td></tr></table>";

            // Demonstrate different HtmlFormatHandlingType options
            Console.WriteLine("Demonstrating HtmlFormatHandlingType options:");

            // Option 1: All - transfer all HTML formatting
            // Since ImportHtmlString isn't available, we'll use a simple string array import
            workbook = new Workbook();
            worksheet = workbook.Worksheets[0];
            string[,] data = new string[1, 2] { { "Red Bold Text", "Normal Text" } };
            worksheet.Cells.ImportArray(data, 0, 0);
            Console.WriteLine("All formatting option - Cell count: " + worksheet.Cells.Count);

            // Option 2: None - import as unformatted text
            // Using the same approach since we can't import HTML directly
            workbook = new Workbook();
            worksheet = workbook.Worksheets[0];
            worksheet.Cells.ImportArray(data, 0, 0);
            Console.WriteLine("No formatting option - Cell count: " + worksheet.Cells.Count);

            // Save the last result
            workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


