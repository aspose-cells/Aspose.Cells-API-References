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
public static void DeleteBlankOptions_Property_EmptyStringAsBlank()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate the worksheet with some data
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

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
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


