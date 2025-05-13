---
title: Worksheet.Workbook
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the workbook object which contains this sheet
type: docs
url: /net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Gets the workbook object which contains this sheet.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
// Called: workbook.CopyTheme(sourceRange.Worksheet.Workbook);
public void Worksheet_Property_Workbook()
{
    var sourceWrkbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsm");
    var sourceRange = sourceWrkbook.Worksheets.GetRangeByName("Alx_PP_Income_Range");

    var workbook = new Workbook();
    workbook.CopyTheme(sourceRange.Worksheet.Workbook);

    var cells = workbook.Worksheets[0].Cells;

    var destRange = cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);
    CopyOptions options = new CopyOptions();

    destRange.Copy(sourceRange, new PasteOptions { OnlyVisibleCells = false, IgnoreLinksToOriginalFile = true });
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].Values, "{100,123.63419862,125.65372708,126.33007859,126.33007859,127.36842105,128.33769945}");
    Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


