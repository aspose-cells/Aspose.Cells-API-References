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
// Called: workbook.Worksheets[0].AutoFitRows();
[Test]
        public void Method_AutoFitRows()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet28269.xls&quot;);
            workbook.Worksheets[0].AutoFitRows();
            Assert.AreEqual(workbook.Worksheets[0].Cells.GetRowHeight(0), 409.5);
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
// Called: sheet.AutoFitRows(true);
[Test]
        public void Method_Boolean_()
        {
            string dir = Constants.sourcePath + &quot;/CELLSNET-44002/&quot;;
            FontConfigs.SetFontFolder(dir + &quot;fonts&quot;, true);

            Workbook wb = new Workbook(dir + &quot;CELLSNET-44002.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[0];
            sheet.AutoFitRows(true);
            Cells cells = sheet.Cells;

            Assert.AreEqual(28, cells.GetRowHeightPixel(0));
            Assert.AreEqual(24, cells.GetRowHeightPixel(9));
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
            Workbook workbook = new Workbook();

            Worksheet sheet = workbook.Worksheets[0];

            Style style = sheet.Cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            style.Font.Name = &quot;DINPro-Regular&quot;;
            style.Font.Size = 8;

            sheet.Cells.Columns[0].Width = 18;

            sheet.Cells[0, 0].SetStyle(style);

            sheet.Cells[0, 0].Value = &quot;Furor-Bet. frei (NG f. KW 10)&quot; + Environment.NewLine +
                &quot;306 ÜN Lena Kern(Mo - So)&quot; + Environment.NewLine +
                Environment.NewLine +
                &quot;Tcherniradev, Overbeck, Kuznick, Ballhaus, Stojanowa, Burmester, Buchwald, Helbig, Schubert, Sählbrandt, Richter, Andreew, Trabichoff, Castagner ab 17:30&quot;;

            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            workbook.Worksheets[0].AutoFitRows(options);
            workbook.Save(Constants.destPath + &quot;CELLSNET47740.xlsx&quot;);
            Assert.AreEqual(195, sheet.Cells.GetRowHeightPixel(0));
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
            testCell.Value = &quot;text&quot;;
            Style cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.BottomBorder, CellBorderType.Double, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[1, 1];
            testCell.Value = &quot;text&quot;;
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.BottomBorder, CellBorderType.MediumDashDot, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[2, 2];
            testCell.Value = &quot;text&quot;;

            testCell = cells[4, 4];
            testCell.Value = &quot;text&quot;;

            testCell = cells[5, 5];
            testCell.Value = &quot;text&quot;;
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thick, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[7, 7];
            testCell.Value = &quot;text&quot;;
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thick, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            testCell = cells[8, 8];
            testCell.Value = &quot;text&quot;;
            cellStyle = testCell.GetStyle();
            cellStyle.SetBorder(BorderType.TopBorder, CellBorderType.Medium, System.Drawing.Color.Black);
            testCell.SetStyle(cellStyle);

            sheet.AutoFitRows(0, 8);
            Assert.AreEqual(18, cells.GetRowHeightPixel(0), &quot;Height of row(0) with ThickBottom border&quot;);
            Assert.AreEqual(19, cells.GetRowHeightPixel(1), &quot;Height of row(1) with ThickTop&amp;MediumBottom border&quot;);
            Assert.AreEqual(17, cells.GetRowHeightPixel(2), &quot;Height of row(2) with MediumTop border&quot;);
            Assert.AreEqual(17, cells.GetRowHeightPixel(3), &quot;Height of row(3) without instance&quot;);
            Assert.AreEqual(18, cells.GetRowHeightPixel(4), &quot;Height of row(4) with ThickBottom border&quot;);
            Assert.AreEqual(18, cells.GetRowHeightPixel(5), &quot;Height of row(5) with ThickTop border&quot;);
            Assert.AreEqual(17, cells.GetRowHeightPixel(6), &quot;Height of row(6) withithout instance&quot;);
            Assert.AreEqual(19, cells.GetRowHeightPixel(7), &quot;Height of row(7) with ThickTop&amp;MidiumBottom border&quot;);
            Assert.AreEqual(17, cells.GetRowHeightPixel(8), &quot;Height of row(8) with MediumTop border&quot;);
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

            Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CellsCloud_1.xlsx&quot;);
            

            Worksheet sheet = wb.Worksheets[&quot;ICE Trip Ticket5&quot;];

            Assert.AreEqual(15,sheet.Cells.GetRowHeight(6));
            sheet.AutoFitRows(6, 6, autoFitterOptions);
            Assert.AreEqual(15, sheet.Cells.GetRowHeight(6));

            wb = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CellsCloud_2.xlsx&quot;);
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


