---
title: HtmlTableLoadOption.Name
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOption property. Get or set the name of table to import from html
type: docs
url: /net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Get or set the name of table to import from html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Examples

```csharp
// Called: Name = &amp;quot;SampleTable&amp;quot;,
public static void Property_Name()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create an instance of HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Create an instance of HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = &quot;table1&quot;,
                Name = &quot;SampleTable&quot;,
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Add the HtmlTableLoadOption to the HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Load the HTML file into the workbook with the specified load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionExample_original.html&quot;, loadOptions);

            // Save the workbook to an Excel file
            workbook.Save(&quot;HtmlTableLoadOptionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


