---
title: Worksheet.AutoFitRow
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits the row height
type: docs
url: /net/aspose.cells/worksheet/autofitrow/
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
// Called: ws.AutoFitRow(0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Style defaultStyle = wb.DefaultStyle;
            defaultStyle.Font.Name = &quot;Arial&quot;;
            defaultStyle.Font.Size = 8;
            wb.DefaultStyle = defaultStyle;
            Worksheet ws = wb.Worksheets[&quot;Sheet1&quot;]; 
            Cells cells = ws.Cells; 
            Cell cell = cells[0, 0];
            cell.PutValue(&quot;Voor meer informatie, nga naar&quot;);
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            ws.AutoFitRow(0);
            wb.Save(Constants.destPath + &quot;Test_159487.xls&quot;);

            Assert.AreEqual(cells.GetRowHeight(0), 33.75,0.01);
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
// Called: worksheet.AutoFitRow(row, column, column);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int row = 0;
            int column = 2;
            Cells cells = worksheet.Cells;
            cells.SetColumnWidthPixel(2, 270);
            Cell cell = cells[row, column];
            // when IndentLevel == 0 this text need 2 rows to display 
            // when IndentLevel == 3 this text need 3 rows to display 
            cell.PutValue(&quot;11111111111111111111111111111 1 1 11111111111111111111111111111 1 1&quot;);
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            style.IndentLevel = 3;
            style.Font.Name = &quot;Courier New&quot;;
            style.Font.Size = 8;
            cell.SetStyle(style);

            worksheet.AutoFitRow(row);
            double incorrectHeight1 = worksheet.Cells.GetRowHeight(row);
            // must be 33.75 but actually is 22.5 
            Assert.AreEqual(incorrectHeight1, 33.75);

            worksheet.AutoFitRow(row, column, column);
            double incorrectHeight2 = worksheet.Cells.GetRowHeight(row);
            // must be 33.75 but actually is 22.5 
            Assert.AreEqual(incorrectHeight1, 33.75);

            style = cell.GetStyle();
            style.IndentLevel = 0;
            cell.SetStyle(style);

            worksheet.AutoFitRow(row);
            double correctHeight1 = worksheet.Cells.GetRowHeight(row);
            // must be 22.5 and actually is 22.5 
            Assert.AreEqual(correctHeight1, 22.5);

            worksheet.AutoFitRow(row, column, column);
            double correctHeight2 = worksheet.Cells.GetRowHeight(row);
            // must be 22.5 and actually is 22.5 
            Assert.AreEqual(correctHeight1, 22.5);
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
[Test]
        public void Method_AutoFitterOptions_()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath +  &quot;CellsNet42476.xlsx&quot;);
            AutoFitterOptions oAutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true, IgnoreHidden = true, OnlyAuto = false };
            double Height = sourceWorkbook.Worksheets[0].Cells.CreateRange(&quot;1:1&quot;).RowHeight;
            sourceWorkbook.Worksheets[0].AutoFitRow(0, 0, 16383, oAutoFitterOptions);
            Height = sourceWorkbook.Worksheets[0].Cells.CreateRange(&quot;1:1&quot;).RowHeight;
            Assert.AreEqual(Height, 15.75);
        }
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

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


