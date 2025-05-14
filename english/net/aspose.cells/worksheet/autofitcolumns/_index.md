---
title: Worksheet.AutoFitColumns
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits all columns in this worksheet
type: docs
url: /net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Autofits all columns in this worksheet.

```csharp
public void AutoFitColumns()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].AutoFitColumns();
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Worksheets[0].AutoFitColumns();
    int w = workbook.Worksheets[0].Cells.GetColumnWidthPixel(0);
    Assert.IsTrue(w == 61 || w == 63 || w == 56);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Autofits all columns in this worksheet.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitting options |

### Examples

```csharp
// Called: workbook.Worksheets[1].AutoFitColumns(options);
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    AutoFitterOptions options = new AutoFitterOptions();
    //   options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
    workbook.Worksheets[1].AutoFitColumns(options);
    Cells cells = workbook.Worksheets[1].Cells;

    int w = cells.GetColumnWidthPixel(14 + 0);
    Assert.IsTrue(w == 48 || w==42 );
    w = cells.GetColumnWidthPixel(14 + 1);
    Assert.IsTrue(w == 27 || w == 29);
    w = cells.GetColumnWidthPixel(14 + 2);
    Assert.IsTrue(w == 41 || w == 36);
    workbook.Save(Constants.destPath  + "example.xlsx");

}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
// Called: sheet.AutoFitColumns(0, 3);
public void Worksheet_Method_AutoFitColumns()
{
    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];

    sheet.AutoFitColumns(0, 3);
    Assert.AreEqual(79, sheet.Cells.GetColumnWidthPixel(0));
    Assert.AreEqual(184, sheet.Cells.GetColumnWidthPixel(1));
    Assert.AreEqual(100, sheet.Cells.GetColumnWidthPixel(2));
    Assert.AreEqual(1822, sheet.Cells.GetColumnWidthPixel(3));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### Remarks

AutoFitColumn is an imprecise function.

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |

### Remarks

AutoFitColumn is an imprecise function.

### Examples

```csharp
// Called: worksheet.AutoFitColumns(18, 3, 78, 52);
public void Worksheet_Method_AutoFitColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFitColumns(18, 3, 78, 52);
    Assert.AreEqual(64,worksheet.Cells.GetColumnWidthPixel(3));
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Autofits the columns width.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |

### Remarks

AutoFitColumn is an imprecise function.

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


