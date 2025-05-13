---
title: Name.GetRange
second_title: Aspose.Cells for .NET API Reference
description: Name method. Gets the range if this name refers to a range
type: docs
url: /net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Gets the range if this name refers to a range.

```csharp
public Range GetRange()
```

### Return Value

The range.

### Examples

```csharp
// Called: Worksheet sheet = name.GetRange().Worksheet;
public void Name_Method_GetRange()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET46465/";


    String namedRng = "Line_Chart_Data";

    Workbook wb = new Workbook(filePath + "InlineCharts.xlsx");

    Name name = wb.Worksheets.Names[namedRng];
    Worksheet sheet = name.GetRange().Worksheet;

    wb.Worksheets.ActiveSheetIndex = sheet.Index;

    Console.WriteLine(sheet.Name);
    Console.WriteLine(name.GetRange().Address);
    sheet.PageSetup.PrintArea = name.GetRange().Address;

    HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
    options.ExportActiveWorksheetOnly = true;
    options.ExportPrintAreaOnly = true;

    wb.Save(CreateFolder(filePath) + "out.xlsx");
    wb.Save(CreateFolder(filePath) + "out.html", options);
}
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Gets the range if this name refers to a range

```csharp
public Range GetRange(bool recalculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |

### Return Value

The range.

### Examples

```csharp
// Called: Aspose.Cells.Range r = name.GetRange(true);
public void Name_Method_GetRange()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 4; i++)
    {
        cells[i, 1].PutValue(i);
    }
    Name name = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
    string fml = "IFERROR(Sheet1!$B$2:$B$4,-1)";
    name.RefersTo = fml;
    cells["C1"].Formula = "=testname";
    cells["D1"].Formula = "SUM(testname)";
    cells["E1"].Formula = fml;
    cells["F1"].Formula = "SUM(" + fml + ")";
    wb.CalculateFormula(false);
    Assert.AreEqual(-1.0, cells["E1"].DoubleValue, "E1");
    Assert.AreEqual(-1.0, cells["F1"].DoubleValue, "E1");
    Assert.AreEqual(1.0, cells["C1"].DoubleValue, "C1");
    Assert.AreEqual(6.0, cells["D1"].DoubleValue, "D1");
    Aspose.Cells.Range r = name.GetRange(true);
    if (r == null || r.FirstRow != 1 || r.FirstColumn != 1 || r.RowCount != 3 || r.ColumnCount != 1)
    {
        Assert.Fail("Name.GetRange should return B2:B4");
    }
    Chart chart = wb.Worksheets[0].Charts[wb.Worksheets[0].Charts.Add(ChartType.Column, 10, 1, 20, 5)];
    chart.NSeries.Add("testname", true);
    Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, "ChartDataCount");
}
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The according sheet index. |
| row | Int32 | The according row index. |
| column | Int32 | The according column index |

### Return Value

The range.

### Examples

```csharp
// Called: Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 1, 1);
public void Name_Method_GetRange()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 1, 1);
    Assert.AreEqual("=Defind!C2:C4", range.RefersTo.Replace("$", ""), "Aspose.Cells.Range.RefersTo");
}
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


