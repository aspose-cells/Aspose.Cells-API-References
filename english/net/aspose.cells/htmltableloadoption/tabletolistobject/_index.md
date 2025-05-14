---
title: HtmlTableLoadOption.TableToListObject
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Indicates whether generate list objects from imported table. The default value is false
type: docs
url: /net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Indicates whether generate list objects from imported table. The default value is false.

```csharp
public bool TableToListObject { get; set; }
```

### Examples

```csharp
// Called: TableToListObject = true
public static void HtmlTableLoadOption_Property_TableToListObject()
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


