---
title: ListColumn.SetCustomTotalsRowFormula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn method. Gets the formula of totals row of this list column
type: docs
url: /net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Gets the formula of totals row of this list column.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | the formula for this list column. |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Examples

```csharp
// Called: lo.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);//.TotalsCalculation = TotalsCalculation.Average;
public void ListColumn_Method_SetCustomTotalsRowFormula()
 {
     Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
     ListObject lo = workbook.Worksheets[0].ListObjects[0];
     lo.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
     lo.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);//.TotalsCalculation = TotalsCalculation.Average;
     workbook.Save(Constants.destPath + "example.xlsx");
     workbook = new Workbook(Constants.destPath + "example.xlsx");
     Assert.AreEqual("=SUM([Column1])", workbook.Worksheets[0].Cells["A4"].Formula);
     Assert.AreEqual("=SUM([Column1])", workbook.Worksheets[0].ListObjects[0].ListColumns[0].GetCustomTotalsRowFormula(false, true));
 }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


