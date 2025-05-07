---
title: FilterColumn.Filter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets and sets the condition of filtering data
type: docs
url: /net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Gets and sets the condition of filtering data.

```csharp
public object Filter { get; set; }
```

### Examples

```csharp
// Called: MultipleFilterCollection fs = fc.Filter as MultipleFilterCollection;
[Test]
     public void Property_Filter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/FilterTest.xlsx");
            AutoFilter filter = workbook.Worksheets[0].AutoFilter;
            filter.MatchBlanks(2);
            filter.MatchNonBlanks(1);
            filter.Refresh();
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsTrue(cells.IsRowHidden(1));
            Assert.IsTrue(cells.IsRowHidden(2));
            Assert.IsTrue(cells.IsRowHidden(3));
            Assert.IsFalse(cells.IsRowHidden(4));
            //workbook.Save(Constants.destPath + "FiterTest.xlsx");
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "FiterTest.xlsx");

            filter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = filter.FilterColumns[2];
            Assert.AreEqual(fc.FilterType, FilterType.MultipleFilters);
            MultipleFilterCollection fs = fc.Filter as MultipleFilterCollection;
            Assert.IsTrue(fs.MatchBlank);
        }
```

### See Also

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


