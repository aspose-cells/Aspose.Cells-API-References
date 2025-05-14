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
// Called: ws.AutoFitColumn(4);
public void Worksheet_Method_AutoFitColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet ws = workbook.Worksheets[0];
    ws.AutoFitColumn(4);
    Assert.AreEqual(11.78, ws.Cells.GetColumnWidth(4));

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


