---
title: Range.FirstColumn
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the index of the first column of the range
type: docs
url: /net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Gets the index of the first column of the range.

```csharp
public int FirstColumn { get; }
```

### Examples

```csharp
// Called: destWorkbook.Worksheets["Sheet1"].Cells.ClearContents(destRange.FirstRow, destRange.FirstColumn,
public void Range_Property_FirstColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    string sourcefileName = Constants.sourcePath  + "example.xlsx";
    string destfileName = Constants.sourcePath  + "example.xlsx";

    var sourceWorkbook = new Workbook(sourcefileName);
    var destWorkbook = new Workbook(destfileName);

    var destRange = destWorkbook.Worksheets["Sheet1"].Cells.CreateRange("A1", "C2");
    var sourceRange = sourceWorkbook.Worksheets["Sheet1"].Cells.CreateRange("A5", "C6");

    destWorkbook.Worksheets["Sheet1"].Cells.ClearContents(destRange.FirstRow, destRange.FirstColumn,
                                                    destRange.FirstRow + destRange.RowCount - 1,
                                                   destRange.FirstColumn + destRange.ColumnCount - 1);

    destRange.CopyData(sourceRange);
    Assert.IsTrue(destRange[0, 0].GetStyle().Font.IsBold);
    destWorkbook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


