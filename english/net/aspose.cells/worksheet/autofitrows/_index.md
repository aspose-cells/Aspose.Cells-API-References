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
// Called: ws.AutoFitRows();
public void Worksheet_Method_AutoFitRows()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47882/";
    string savePath = CreateFolder(filePath);

    string bgresult = System.IO.File.ReadAllText(filePath + "HtmlPage9.html");
    using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(bgresult)))
    {
        HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.Html);
        options.AutoFitColsAndRows = true;//IF WE COMMENT THIS LINE, THE CODE WORKS FINE

        Workbook wb = new Workbook(stream, options);

        Worksheet ws = wb.Worksheets[0];
        ws.Name = "Test";
        ws.AutoFitRows();
        ws.AutoFitColumns();

        PageSetup pageSetup = ws.PageSetup;
        pageSetup.SetHeader(1, string.Format("&\"Times New Roman,Bold\"Title: {0} {1} {2}", "Test BillingGuide Name", "Enabled", DateTime.Now.ToString("yyyy-mm-dd")));

        wb.Save(savePath + "HtmlPage9.xlsx", SaveFormat.Xlsx);
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
public void Worksheet_Method_AutoFitRows()
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
// Called: worksheet.AutoFitRows(new AutoFitterOptions
private static void Worksheet_Method_AutoFitRows(Worksheet worksheet)
        {
            worksheet.AutoFitRows(new AutoFitterOptions
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
public void Worksheet_Method_AutoFitRows()
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
        public void Worksheet_Method_AutoFitRows()
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


