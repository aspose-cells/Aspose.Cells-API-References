---
title: PivotShowValuesSetting.CalculationType
second_title: Aspose.Cells for .NET API Reference
description: PivotShowValuesSetting property. Represents how to show values of a data field in the pivot report
type: docs
url: /net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Represents how to show values of a data field in the pivot report.

```csharp
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.DataFields[1].ShowValuesSetting.CalculationType, PivotFieldDataDisplayFormat.RankLargestToSmallest);
public void PivotShowValuesSetting_Property_CalculationType()
{
    var wb = new Workbook(Constants.openPivottablePath + "testDisplayFormat.xlsx");
    PivotTable pt = wb.Worksheets[1].PivotTables[0];
    //Console.WriteLine(pt.PageFieldWrapCount);
    //Console.WriteLine(pt.DisplayNullString);
    //Console.WriteLine(pt.PreserveFormatting);
    //Console.WriteLine(pt.ItemPrintTitles);
    Assert.AreEqual(pt.DataFields[1].ShowValuesSetting.CalculationType, PivotFieldDataDisplayFormat.RankLargestToSmallest);
    wb.Save(Constants.savePivottablePath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


