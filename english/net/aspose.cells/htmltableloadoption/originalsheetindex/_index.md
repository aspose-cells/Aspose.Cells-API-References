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
// Called: option.OriginalSheetIndex = 0;
public static void Property_OriginalSheetIndex()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add(&quot;tableId&quot;);

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add(&quot;tableId2&quot;, 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add(&quot;tableId3&quot;, 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = &quot;tableId&quot;;
            option.Name = &quot;TableName&quot;;
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook(&quot;HtmlTableLoadOptionCollectionExample_original.html&quot;, loadOptions);

            // Save the workbook
            workbook.Save(&quot;HtmlTableLoadOptionCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


