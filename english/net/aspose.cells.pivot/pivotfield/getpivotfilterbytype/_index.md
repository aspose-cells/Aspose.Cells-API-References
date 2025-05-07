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
            var wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET57201macro.xlsm");
            PivotFilter filter = wb.Worksheets[1].PivotTables[0].RowFields[0].GetPivotFilterByType(PivotFilterType.Count);
           Assert.AreEqual(PivotFilterType.Count,filter.FilterType);
            Assert.AreEqual(3,filter.ValueFieldIndex);
            Assert.AreEqual("1",filter.Value1);
            wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET-57201.xlsm");
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            table.BaseFields[1].FilterTop10(0, PivotFilterType.Count, true, 1);
            table.BaseFields[1].FilterByLabel(PivotFilterType.CaptionGreaterThan, "1", null);
            Assert.AreEqual(2,table.BaseFields[1].GetFilters().Length);
            table.BaseFields[0].FilterTop10(0, PivotFilterType.Count, true, 10);

            wb.Save(Constants.PivotTableDestPath + "CELLSNET-57201.xlsx");
            wb = new Workbook(Constants.PivotTableDestPath + "CELLSNET-57201.xlsx");
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


