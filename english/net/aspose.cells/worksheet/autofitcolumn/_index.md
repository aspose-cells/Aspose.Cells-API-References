---
title: Worksheet.AutoFitColumn
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits the column width
type: docs
url: /net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Autofits the column width.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| firstRow | Int32 | First row index. |
| lastRow | Int32 | Last row index. |

### Remarks

This method autofits a row based on content in a range of cells within the row.

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Autofits the column width.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
// Called: range.Worksheet.AutoFitColumn(range.FirstColumn + i);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET48473.xlsx");
            //Console.WriteLine(workbook.Worksheets[0].Cells.MaxRow);
            var sheet = workbook.Worksheets[0];
            var range = sheet.Workbook.Worksheets.GetRangeByName("DataRange");

            for (int i = 0; i < range.ColumnCount; i++)
            {
                range.Worksheet.AutoFitColumn(range.FirstColumn + i);
            }
            Assert.AreEqual(26,sheet.Cells.GetColumnWidthPixel(2));
            workbook.Save(Constants.destPath + "CELLSNET48473.xlsx");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


