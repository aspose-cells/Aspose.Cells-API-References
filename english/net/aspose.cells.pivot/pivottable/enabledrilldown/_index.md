---
title: PivotTable.EnableDrilldown
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets whether drilldown is enabled
type: docs
url: /net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Gets whether drilldown is enabled.

```csharp
public bool EnableDrilldown { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.EnableDrilldown, true);
[Test]
        public void Property_EnableDrilldown()
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
            //wb.Save("D:\\40095.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


