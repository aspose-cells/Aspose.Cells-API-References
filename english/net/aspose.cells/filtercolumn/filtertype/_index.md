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

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


