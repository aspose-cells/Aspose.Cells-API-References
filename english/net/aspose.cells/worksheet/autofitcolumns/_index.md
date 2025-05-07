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
[Test]
        public void Method_AutoFitColumns()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-42339.xlsx");
            workbook.Worksheets[0].AutoFitColumns();
            Assert.AreEqual(workbook.Worksheets[0].Cells.GetColumnWidthPixel(0), 93);
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
// Called: worksheet.AutoFitColumns(new AutoFitterOptions
private static void Method_AutoFitterOptions_(Worksheet worksheet)
        {
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = int.MaxValue,
                OnlyAuto = true
            });

            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = int.MaxValue,
                OnlyAuto = true
            });
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
[Test]
        public void Method_Int32_()
        {
            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CELLSNET52968.xlsx");
            Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];

            sheet.AutoFitColumns(0, 3);
            Assert.AreEqual(79, sheet.Cells.GetColumnWidthPixel(0));
            Assert.AreEqual(184, sheet.Cells.GetColumnWidthPixel(1));
            Assert.AreEqual(100, sheet.Cells.GetColumnWidthPixel(2));
            Assert.AreEqual(1822, sheet.Cells.GetColumnWidthPixel(3));
            workbook.Save(Constants.destPath + "CELLSNET52968.xlsx");
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
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET51760.xlsx");
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


