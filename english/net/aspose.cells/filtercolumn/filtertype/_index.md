---
title: FilterColumn.FilterType
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets and sets the type fo filtering data
type: docs
url: /net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Gets and sets the type fo filtering data.

```csharp
public FilterType FilterType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(fc.FilterType, FilterType.MultipleFilters);
[Test]
        public void Property_FilterType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;AutoFilter/DateFilter01.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[&quot;Sheet1&quot;];

            Assert.IsTrue(sheet.Cells.IsBlankColumn(2));
            Assert.IsFalse(sheet.Cells.IsBlankColumn(1));
            sheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
           Assert.IsTrue(sheet.Cells.IsRowHidden(1));
            Assert.IsFalse(sheet.Cells.IsRowHidden(2));
            Assert.IsTrue(sheet.Cells.IsRowHidden(3));
            //wb.Save(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            sheet = wb.Worksheets[&quot;Sheet1&quot;];
            AutoFilter filter = wb.Worksheets[0].AutoFilter;
            FilterColumn fc = filter.FilterColumns[1];
            Assert.AreEqual(fc.FilterType, FilterType.MultipleFilters);
            MultipleFilterCollection m = fc.Filter as MultipleFilterCollection;
            DateTimeGroupItem dateTimeGroupItem = m[0] as DateTimeGroupItem;
            Assert.AreEqual(dateTimeGroupItem.Day, 7);
            filter.RemoveDateFilter(1, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            Assert.AreEqual(m.Count, 0);
            filter.RemoveFilter(1);
            filter.Refresh(true);
            Assert.IsFalse(sheet.Cells.IsRowHidden(1));
            Assert.IsFalse(sheet.Cells.IsRowHidden(2));
            Assert.IsFalse(sheet.Cells.IsRowHidden(3));
            //wb.Save(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            filter = wb.Worksheets[0].AutoFilter;
            filter.DynamicFilter(1, DynamicFilterType.September);
            fc = filter.FilterColumns[1];
            //wb.Save(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;DateFilter01.xlsx&quot;);
            filter = wb.Worksheets[0].AutoFilter;
            fc = filter.FilterColumns[1];
            Assert.AreEqual(fc.FilterType, FilterType.DynamicFilter);
        }
```

### See Also

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


