---
title: PivotField.ShowValuesSetting
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the settings of showing values as when the ShowDataAs calculation is in use
type: docs
url: /net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Gets the settings of showing values as when the ShowDataAs calculation is in use.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.DataFields[1].ShowValuesSetting.CalculationType, PivotFieldDataDisplayFormat.RankLargestToSmallest);
[Test]
        public void Property_ShowValuesSetting()
        {
            var wb = new Workbook(Constants.openPivottablePath + &quot;testDisplayFormat.xlsx&quot;);
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            //Console.WriteLine(pt.PageFieldWrapCount);
            //Console.WriteLine(pt.DisplayNullString);
            //Console.WriteLine(pt.PreserveFormatting);
            //Console.WriteLine(pt.ItemPrintTitles);
            Assert.AreEqual(pt.DataFields[1].ShowValuesSetting.CalculationType, PivotFieldDataDisplayFormat.RankLargestToSmallest);
            wb.Save(Constants.savePivottablePath + &quot;40095.xlsx&quot;);
        }
```

### See Also

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


