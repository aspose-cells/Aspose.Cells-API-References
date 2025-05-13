---
title: PivotField.AutoShowCount
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represent the number of top or bottom items that are automatically shown in the specified PivotTable field
type: docs
url: /net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

```csharp
public int AutoShowCount { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.RowFields[0].AutoShowCount, 2);
public void PivotField_Property_AutoShowCount()
{
    var wb = new Workbook(Constants.openPivottablePath + "testCount.xlsx");
    PivotTable pt = wb.Worksheets[1].PivotTables[0];
    //Console.WriteLine(pt.PageFieldWrapCount);
    //Console.WriteLine(pt.DisplayNullString);
    //Console.WriteLine(pt.PreserveFormatting);
    //Console.WriteLine(pt.ItemPrintTitles);
    Assert.AreEqual(pt.RowFields[0].AutoShowCount, 2);

    wb = new Workbook(Constants.openPivottablePath + "testCount(1).xls");
    pt = wb.Worksheets[1].PivotTables[0];
    //Console.WriteLine(pt.PageFieldWrapCount);
    //Console.WriteLine(pt.DisplayNullString);
    //Console.WriteLine(pt.PreserveFormatting);
    //Console.WriteLine(pt.ItemPrintTitles);
    Assert.AreEqual(pt.RowFields[0].AutoShowCount, 2);

    wb = new Workbook(Constants.openPivottablePath + "testCount(2).xls");
    pt = wb.Worksheets[1].PivotTables[0];
    //Console.WriteLine(pt.PageFieldWrapCount);
    //Console.WriteLine(pt.DisplayNullString);
    //Console.WriteLine(pt.PreserveFormatting);
    //Console.WriteLine(pt.ItemPrintTitles);
    Assert.AreEqual(pt.EnableDrilldown, true);
    //wb.Save("example.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


