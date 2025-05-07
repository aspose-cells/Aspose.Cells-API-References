---
title: Worksheet.SelectRange
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Selects a range
type: docs
url: /net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Selects a range.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| totalRows | Int32 | The number of rows. |
| totalColumns | Int32 | The number of columns |
| removeOthers | Boolean | True means removing other selected range and only select this range. |

### Examples

```csharp
// Called: workbook.Worksheets[0].SelectRange(1, 1, 2, 2, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SRange01.xlsx");
            Aspose.Cells.Range[] rs = workbook.Worksheets[0].GetSelectedAreas();
            Assert.AreEqual(2, rs.Length);
            workbook.Worksheets[0].SelectRange(1, 1, 2, 2, true);
            rs = workbook.Worksheets[0].GetSelectedAreas();
            Assert.AreEqual(1, rs.Length);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


