---
title: Class DeleteBlankOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.DeleteBlankOptions class. Represents the setting of deleting blank cells/rows/columns
type: docs
url: /net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Gets/sets the monitor for tracking changes caused by the deletion.(Inherited from [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Indicates how to process merged cells when deleting blank rows/columns. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Specifies the start row/column index of the range to check and delete blank row/column. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indicates if update references in other worksheets.(Inherited from [`DeleteOptions`](../deleteoptions/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
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
    }
}
```

### See Also

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


