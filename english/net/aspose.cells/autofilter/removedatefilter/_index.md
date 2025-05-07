---
title: AutoFilter.RemoveDateFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Removes a date filter
type: docs
url: /net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Removes a date filter.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | DateTimeGroupingType | The grouping type |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |
| hour | Int32 | The hour. |
| minute | Int32 | The minute. |
| second | Int32 | The second. |

### Remarks

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

### Examples

```csharp
// Called: filter.RemoveDateFilter(1, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/DateFilter01.xlsx");
            Worksheet sheet = wb.Worksheets["Sheet1"];

            Assert.IsTrue(sheet.Cells.IsBlankColumn(2));
            Assert.IsFalse(sheet.Cells.IsBlankColumn(1));
            sheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
           Assert.IsTrue(sheet.Cells.IsRowHidden(1));
            Assert.IsFalse(sheet.Cells.IsRowHidden(2));
            Assert.IsTrue(sheet.Cells.IsRowHidden(3));
            //wb.Save(Constants.destPath + "DateFilter01.xlsx");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "DateFilter01.xlsx");
            sheet = wb.Worksheets["Sheet1"];
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
            //wb.Save(Constants.destPath + "DateFilter01.xlsx");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "DateFilter01.xlsx");
            filter = wb.Worksheets[0].AutoFilter;
            filter.DynamicFilter(1, DynamicFilterType.September);
            fc = filter.FilterColumns[1];
            //wb.Save(Constants.destPath + "DateFilter01.xlsx");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "DateFilter01.xlsx");
            filter = wb.Worksheets[0].AutoFilter;
            fc = filter.FilterColumns[1];
            Assert.AreEqual(fc.FilterType, FilterType.DynamicFilter);
        }
```

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


