---
title: ListColumn.TotalsCalculation
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the type of calculation in the Totals row of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Gets and sets the type of calculation in the Totals row of the list column.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Examples

```csharp
// Called: lo.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
[Test]
       public void Property_TotalsCalculation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet49990.xlsx");
            ListObject lo = workbook.Worksheets[0].ListObjects[0];
            lo.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            lo.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);//.TotalsCalculation = TotalsCalculation.Average;
            workbook.Save(Constants.destPath + "CellsNet49990.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet49990.xlsx");
            Assert.AreEqual("=SUM([Column1])", workbook.Worksheets[0].Cells["A4"].Formula);
            Assert.AreEqual("=SUM([Column1])", workbook.Worksheets[0].ListObjects[0].ListColumns[0].GetCustomTotalsRowFormula(false, true));
        }
```

### See Also

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


