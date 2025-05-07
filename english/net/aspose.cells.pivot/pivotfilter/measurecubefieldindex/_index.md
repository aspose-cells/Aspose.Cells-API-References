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
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET-53133.xlsx");
            PivotTable pt = workbook.Worksheets["Liefertreue Top 10 Abteilungen"].PivotTables[0];
            Assert.AreEqual(19, pt.BaseFields[1].GetFilters()[0].MeasureCubeFieldIndex);
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET53133.xlsx");
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + "CELLSNET53133.xlsx", "xl/pivotTables/pivotTable1.xml", new string[] { "iMeasureHier=\"19\"" }, true));
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


