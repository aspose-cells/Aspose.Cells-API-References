---
title: HtmlTableLoadOption.TableIndex
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Get or set the index of table to import from html
type: docs
url: /net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Get or set the index of table to import from html.

```csharp
public int TableIndex { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HTML load options
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Configure table load option with TableIndex = 0 (first table)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Add the table load option
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Load HTML file (replace with actual path)
            workbook = new Workbook("input.html", loadOptions);

            // Save as Excel file
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


