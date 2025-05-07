---
title: FilterColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FilterColumnCollection property. Gets FilterColumn object at the special field
type: docs
url: /net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Gets [`FilterColumn`](../../filtercolumn/) object at the special field.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parameter | Description |
| --- | --- |
| fieldIndex | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Return Value

Returns [`FilterColumn`](../../filtercolumn/) object.

### Examples

```csharp
// Called: FilterColumn fc = filter.FilterColumns[2];
[Test]
     public void Property_Int32_()
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

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


