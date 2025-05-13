---
title: Worksheet.AutoFitRow
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits row height in a rectangle range
type: docs
url: /net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Autofits row height in a rectangle range.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Autofits the row height.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |

### Remarks

AutoFitRow is an imprecise function.

### Examples

```csharp
// Called: w1.Worksheets[0].AutoFitRow(0);
public void Worksheet_Method_AutoFitRow()
{
    Workbook w1 = new Workbook();
   Assert.AreEqual(12.75,w1.Worksheets[0].Cells.StandardHeight);
    Style style = w1.Worksheets[0].Cells["A1"].GetStyle();
    style.IsTextWrapped = (true);
    w1.Worksheets[0].Cells["A1"].SetStyle(style);
    w1.Worksheets[0].Cells["A1"].Value = ("LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT");
    w1.Worksheets[0].Cells["A2"].Value = ("SOME OTHER LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT");
    w1.Worksheets[0].AutoFitRow(0);
    Assert.AreEqual(12.75, w1.Worksheets[0].Cells.StandardHeight);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Autofits the row height.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |

### Remarks

This method autofits a row based on content in a range of cells within the row.

### Examples

```csharp
// Called: wb.Worksheets[0].AutoFitRow(2, 8, 8);
public void Worksheet_Method_AutoFitRow()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(299, wb.Worksheets[0].Cells.GetColumnWidthPixel(8));
    wb.Worksheets[0].AutoFitRow(2, 8, 8);
    Assert.AreEqual(112.5, wb.Worksheets[0].Cells.GetRowHeight(2));
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Autofits the row height.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitter options |

### Remarks

This method autofits a row based on content in a range of cells within the row.

### Examples

```csharp
// Called: sourceWorkbook.Worksheets[0].AutoFitRow(0, 0, 16383, oAutoFitterOptions);
public void Worksheet_Method_AutoFitRow()
{
    Workbook sourceWorkbook = new Workbook(Constants.sourcePath +  "example.xlsx");
    AutoFitterOptions oAutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true, IgnoreHidden = true, OnlyAuto = false };
    double Height = sourceWorkbook.Worksheets[0].Cells.CreateRange("1:1").RowHeight;
    sourceWorkbook.Worksheets[0].AutoFitRow(0, 0, 16383, oAutoFitterOptions);
    Height = sourceWorkbook.Worksheets[0].Cells.CreateRange("1:1").RowHeight;
    Assert.AreEqual(Height, 15.75);
}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


