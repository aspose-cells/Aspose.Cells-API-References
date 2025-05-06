---
title: PivotFilter.MeasureCubeFieldIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply
type: docs
url: /net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(19, pt.BaseFields[1].GetFilters()[0].MeasureCubeFieldIndex);
[Test]
        public void Property_MeasureCubeFieldIndex()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET-53133.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[&quot;Liefertreue Top 10 Abteilungen&quot;].PivotTables[0];
            Assert.AreEqual(19, pt.BaseFields[1].GetFilters()[0].MeasureCubeFieldIndex);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET53133.xlsx&quot;);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + &quot;CELLSNET53133.xlsx&quot;, &quot;xl/pivotTables/pivotTable1.xml&quot;, new string[] { &quot;iMeasureHier=\&quot;19\&quot;&quot; }, true));
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


