---
title: Cells.IsBlankColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether given column is blankdoes not contain any data
type: docs
url: /net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Checks whether given column is blank(does not contain any data).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | the column index |

### Return Value

true if given column does not contain any data

### Examples

```csharp
// Called: Assert.IsFalse(sheet.Cells.IsBlankColumn(1));
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

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


