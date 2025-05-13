---
title: Range.ColumnCount
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the count of columns in the range
type: docs
url: /net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Gets the count of columns in the range.

```csharp
public int ColumnCount { get; }
```

### Examples

```csharp
// Called: for (int i = 0; i < range.ColumnCount; i++)
public void Range_Property_ColumnCount()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //Console.WriteLine(workbook.Worksheets[0].Cells.MaxRow);
    var sheet = workbook.Worksheets[0];
    var range = sheet.Workbook.Worksheets.GetRangeByName("DataRange");

    for (int i = 0; i < range.ColumnCount; i++)
    {
        range.Worksheet.AutoFitColumn(range.FirstColumn + i);
    }
    Assert.AreEqual(26,sheet.Cells.GetColumnWidthPixel(2));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


