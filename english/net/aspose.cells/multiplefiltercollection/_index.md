---
title: Class MultipleFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MultipleFilterCollection class. Represents the multiple filter collection
type: docs
url: /net/aspose.cells/multiplefiltercollection/
---
## MultipleFilterCollection class

Represents the multiple filter collection.

```csharp
public class MultipleFilterCollection : CollectionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [MultipleFilterCollection](multiplefiltercollection/)() | Constructs one new instance. |

## Properties

| Name | Description |
| --- | --- |
| [Item](../../aspose.cells/multiplefiltercollection/item/) { get; } | DateTimeGroupItem or a simple object. |
| [MatchBlank](../../aspose.cells/multiplefiltercollection/matchblank/) { get; set; } | Indicates whether to filter by blank. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/multiplefiltercollection/add/)(string) | Adds string filter. |

### Examples

```csharp
// Called: MultipleFilterCollection m = fc.Filter as MultipleFilterCollection;
[Test]
        public void Type_MultipleFilterCollection()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


