---
title: ListColumn.GetCustomTotalsRowFormula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn method. Gets the formula of totals row of this list column
type: docs
url: /net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

Gets the formula of totals row of this list column.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

The formula of this list column.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;=SUM([Column1])&amp;quot;, workbook.Worksheets[0].ListObjects[0].ListColumns[0].GetCustomTotalsRowFormula(false, true));
[Test]
       public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet49990.xlsx&quot;);
            ListObject lo = workbook.Worksheets[0].ListObjects[0];
            lo.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            lo.ListColumns[0].SetCustomTotalsRowFormula(&quot;=SUM([Column1])&quot;, false, false);//.TotalsCalculation = TotalsCalculation.Average;
            workbook.Save(Constants.destPath + &quot;CellsNet49990.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet49990.xlsx&quot;);
            Assert.AreEqual(&quot;=SUM([Column1])&quot;, workbook.Worksheets[0].Cells[&quot;A4&quot;].Formula);
            Assert.AreEqual(&quot;=SUM([Column1])&quot;, workbook.Worksheets[0].ListObjects[0].ListColumns[0].GetCustomTotalsRowFormula(false, true));
        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


