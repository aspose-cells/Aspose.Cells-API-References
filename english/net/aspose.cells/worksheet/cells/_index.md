---
title: Worksheet.Cells
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the Cells collection
type: docs
url: /net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Gets the `Cells` collection.

```csharp
public Cells Cells { get; }
```

### Examples

```csharp
// Called: Cells cells = workbook.Worksheets[0].Cells;
[Test]
        public void Property_Cells()
        {
            caseName = &quot;testDeleteRangeFormual_023&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual3.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRange(1, 2, 2, 5, ShiftType.Left);

            checkDeleteRangeFormual_023(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkDeleteRangeFormual_023(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkDeleteRangeFormual_023(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkDeleteRangeFormual_023(workbook);
            Util.SaveAsBuffer(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


