---
title: DeleteBlankOptions.EmptyStringAsBlank
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Whether one cell will be taken as blank when its value is empty string. Default value is true
type: docs
url: /net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Whether one cell will be taken as blank when its value is empty string. Default value is true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Examples

```csharp
// Called: EmptyStringAsBlank = true,
public static void Property_EmptyStringAsBlank()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate the worksheet with some data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Data&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;More Data&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;&quot;);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Even More Data&quot;);

            // Create an instance of DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Delete blank rows based on the options
            worksheet.Cells.DeleteBlankRows(options);

            // Save the workbook
            workbook.Save(&quot;DeleteBlankOptionsExample.xlsx&quot;);
            workbook.Save(&quot;DeleteBlankOptionsExample.pdf&quot;);
            return;
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


