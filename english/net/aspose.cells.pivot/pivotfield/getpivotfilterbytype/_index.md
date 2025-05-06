---
title: PivotField.GetPivotFilterByType
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets the pivot filter of the pivot field by type
type: docs
url: /net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

Gets the pivot filter of the pivot field by type

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### Examples

```csharp
// Called: PivotFilter filter = wb.Worksheets[1].PivotTables[0].RowFields[0].GetPivotFilterByType(PivotFilterType.Count);
[Test]
        public void Method_PivotFilterType_()
        {
            var wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET57201macro.xlsm&quot;);
            PivotFilter filter = wb.Worksheets[1].PivotTables[0].RowFields[0].GetPivotFilterByType(PivotFilterType.Count);
           Assert.AreEqual(PivotFilterType.Count,filter.FilterType);
            Assert.AreEqual(3,filter.ValueFieldIndex);
            Assert.AreEqual(&quot;1&quot;,filter.Value1);
            wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET-57201.xlsm&quot;);
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            table.BaseFields[1].FilterTop10(0, PivotFilterType.Count, true, 1);
            table.BaseFields[1].FilterByLabel(PivotFilterType.CaptionGreaterThan, &quot;1&quot;, null);
            Assert.AreEqual(2,table.BaseFields[1].GetFilters().Length);
            table.BaseFields[0].FilterTop10(0, PivotFilterType.Count, true, 10);

            wb.Save(Constants.PivotTableDestPath + &quot;CELLSNET-57201.xlsx&quot;);
            wb = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET-57201.xlsx&quot;);
            table = wb.Worksheets[1].PivotTables[0];
            Assert.AreEqual(2, table.BaseFields[1].GetFilters().Length);
            Assert.AreEqual(PivotFilterType.Count, table.BaseFields[0].GetFilters()[0].FilterType);

        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


