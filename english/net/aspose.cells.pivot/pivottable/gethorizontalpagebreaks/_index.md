---
title: PivotTable.GetHorizontalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets horizontal page breaks of this pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Gets horizontal page breaks of this pivot table.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Examples

```csharp
// Called: int[] rows = pivot.GetHorizontalPageBreaks();
public void PivotTable_Method_GetHorizontalPageBreaks()
{
    Workbook wb = new Workbook(Constants.sourcePath + "pivot_pagebreaks.xlsx");
    PivotTable pivot = wb.Worksheets[1].PivotTables[0];
    pivot.RefreshData();
    pivot.CalculateData();
    int[] rows = pivot.GetHorizontalPageBreaks();

    Assert.AreEqual(2, rows.Length);
    Assert.AreEqual(11, rows[0]);
    Assert.AreEqual(15, rows[1]);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


