---
title: HtmlTableLoadOption.OriginalSheetIndex
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Get or set the original index of worksheet in the html
type: docs
url: /net/aspose.cells/htmltableloadoption/originalsheetindex/
---
## HtmlTableLoadOption.OriginalSheetIndex property

Get or set the original index of worksheet in the html.

```csharp
public int OriginalSheetIndex { get; set; }
```

### Examples

```csharp
// Called: OriginalSheetIndex = 0,
public static void HtmlTableLoadOption_Property_OriginalSheetIndex()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create an instance of HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Create an instance of HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Add the HtmlTableLoadOption to the HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Load the HTML file into the workbook with the specified load options
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Save the workbook to an Excel file
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


