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
// Called: workbook.Worksheets[0].SelectRange(1, 1, 5, 5,true);
public void Worksheet_Method_SelectRange()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].SelectRange(1, 1, 5, 5,true);
    Assert.AreEqual(workbook.Worksheets[0].ActiveCell, "B2");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


