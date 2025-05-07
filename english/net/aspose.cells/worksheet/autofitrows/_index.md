---
title: Worksheet.AutoFitRows
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Autofits all rows in this worksheet
type: docs
url: /net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows() {#autofitrows}

Autofits all rows in this worksheet.

```csharp
public void AutoFitRows()
```

### Examples

```csharp
// Called: sheet.AutoFitRows();
[Test]
        public void Method_AutoFitRows()
        {
            using (var workbook = new Workbook(Constants.sourcePath + "CELLSNET-46799.xlsx"))
            {
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    sheet.AutoFitColumns();
                    sheet.AutoFitRows();
                }
                Aspose.Cells.PdfSaveOptions _options = new Aspose.Cells.PdfSaveOptions();
                workbook.Save(Constants.destPath + "CellsNet46799.pdf", _options);
            }
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Autofits all rows in this worksheet.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | Boolean | True,only autofits the row height when row height is not customed. |

### Examples

```csharp
// Called: workbook.Worksheets[1].AutoFitRows(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "new_fangled_spreadsheet.xls");
            workbook.Worksheets[1].AutoFitRows(true);
            Assert.AreEqual(workbook.Worksheets[1].Cells.GetRowHeight(131), 276.1);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Autofits all rows in this worksheet.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitter options |

### Examples

```csharp
// Called: workbook.Worksheets[0].AutoFitRows(options);
[Test]
        public void Method_AutoFitterOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42777_1.xlsx");
            AutoFitterOptions options = new AutoFitterOptions();

            options.AutoFitMergedCells = (true);
            // Set auto-fit for merged cells
            //options.setAutoFitMergedCells(true);
            workbook.Worksheets[0].AutoFitRows(options);
            Assert.AreEqual(18, workbook.Worksheets[0].Cells.GetRowHeightPixel(11));
            workbook.Save(Constants.destPath + "CELLSJAVA42777_1.xlsx");
        }
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int) {#autofitrows_3}

Autofits row height in a range.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |

### Examples

```csharp
// Called: sheet.AutoFitRows(0, 8);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            Cell testCell = cells[0, 0];
            testCell.Value = "text";
            Style cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.BottomBorder, CellBorderType.Double, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[1, 1];
            testCell.Value = "text";
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.BottomBorder, CellBorderType.MediumDashDot, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[2, 2];
            testCell.Value = "text";

            testCell = cells[4, 4];
            testCell.Value = "text";

            testCell = cells[5, 5];
            testCell.Value = "text";
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thick, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[7, 7];
            testCell.Value = "text";
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thick, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[8, 8];
            testCell.Value = "text";
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Medium, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            sheet.AutoFitRows(0, 8);
            Assert.AreEqual(18, cells.GetRowHeightPixel(0), "Height of row(0) with ThickBottom border");
            Assert.AreEqual(19, cells.GetRowHeightPixel(1), "Height of row(1) with ThickTop&MediumBottom border");
            Assert.AreEqual(17, cells.GetRowHeightPixel(2), "Height of row(2) with MediumTop border");
            Assert.AreEqual(17, cells.GetRowHeightPixel(3), "Height of row(3) without instance");
            Assert.AreEqual(18, cells.GetRowHeightPixel(4), "Height of row(4) with ThickBottom border");
            Assert.AreEqual(18, cells.GetRowHeightPixel(5), "Height of row(5) with ThickTop border");
            Assert.AreEqual(17, cells.GetRowHeightPixel(6), "Height of row(6) withithout instance");
            Assert.AreEqual(19, cells.GetRowHeightPixel(7), "Height of row(7) with ThickTop&MidiumBottom border");
            Assert.AreEqual(17, cells.GetRowHeightPixel(8), "Height of row(8) with MediumTop border");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Autofits row height in a range.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| options | AutoFitterOptions | The options of auto fitter. |

### Examples

```csharp
// Called: sheet.AutoFitRows(6, 6, autoFitterOptions);
[Test]
        public void Method_AutoFitterOptions_()
        {
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.OnlyAuto = true;

            Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsCloud_1.xlsx");
            

            Worksheet sheet = wb.Worksheets["ICE Trip Ticket5"];

            Assert.AreEqual(15,sheet.Cells.GetRowHeight(6));
            sheet.AutoFitRows(6, 6, autoFitterOptions);
            Assert.AreEqual(15, sheet.Cells.GetRowHeight(6));

            wb = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsCloud_2.xlsx");
            wb.Worksheets[0].AutoFitRows();
#if !NETCOREAPP2_0
            Assert.AreEqual(42.75, wb.Worksheets[0].Cells.GetRowHeight(0));
#endif
        }
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


