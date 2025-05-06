---
title: PivotFilter.UseWholeDay
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Indicates whether uses whole days in its filtering criteria
type: docs
url: /net/aspose.cells.pivot/pivotfilter/usewholeday/
---
## PivotFilter.UseWholeDay property

Indicates whether uses whole days in its filtering criteria.

```csharp
public bool UseWholeDay { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
[Test]
        public void Property_UseWholeDay()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET57204.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET57204.xlsb&quot;);
        
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET57204.xlsb&quot;);
            pt = workbook.Worksheets[0].PivotTables[0];
            Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET57204.xlsx&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET57204.xlsx&quot;);
            pt = workbook.Worksheets[0].PivotTables[0];
            Assert.IsTrue(pt.BaseFields[1].GetFilters()[0].UseWholeDay);
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


