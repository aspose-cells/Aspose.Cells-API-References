---
title: PivotFilter.GetDateTimeValues
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter method. Gets values of the number filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/getdatetimevalues/
---
## PivotFilter.GetDateTimeValues method

Gets values of the number filter.

```csharp
public DateTime[] GetDateTimeValues()
```

### Examples

```csharp
// Called: Assert.AreEqual(DateTime.Now.AddDays(1).Day, filter.GetDateTimeValues()[1].Day);
[Test]
        public void Method_GetDateTimeValues()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET57202.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.BaseFields[1].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET57202.xlsx&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET57202.xlsx&quot;);
            pt = workbook.Worksheets[0].PivotTables[0];
            Assert.AreEqual(1, pt.BaseFields[1].GetFilters().Length);
            PivotFilter filter = pt.BaseFields[1].GetFilters()[0];
            Assert.AreEqual(PivotFilterType.DateBetween, filter.FilterType);
            Assert.AreEqual(DateTime.Now.Day, filter.GetDateTimeValues()[0].Day);
            Assert.AreEqual(DateTime.Now.AddDays(1).Day, filter.GetDateTimeValues()[1].Day);
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


