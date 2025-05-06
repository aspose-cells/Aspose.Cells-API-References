---
title: MultipleFilterCollection.MatchBlank
second_title: Aspose.Cells for .NET API Reference
description: MultipleFilterCollection property. Indicates whether to filter by blank
type: docs
url: /net/aspose.cells/multiplefiltercollection/matchblank/
---
## MultipleFilterCollection.MatchBlank property

Indicates whether to filter by blank.

```csharp
public bool MatchBlank { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(fs.MatchBlank);
[Test]
     public void Property_MatchBlank()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/FilterTest.xlsx&quot;);
            AutoFilter filter = workbook.Worksheets[0].AutoFilter;
            filter.MatchBlanks(2);
            filter.MatchNonBlanks(1);
            filter.Refresh();
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsTrue(cells.IsRowHidden(1));
            Assert.IsTrue(cells.IsRowHidden(2));
            Assert.IsTrue(cells.IsRowHidden(3));
            Assert.IsFalse(cells.IsRowHidden(4));
            //workbook.Save(Constants.destPath + &quot;FiterTest.xlsx&quot;);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;FiterTest.xlsx&quot;);

            filter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = filter.FilterColumns[2];
            Assert.AreEqual(fc.FilterType, FilterType.MultipleFilters);
            MultipleFilterCollection fs = fc.Filter as MultipleFilterCollection;
            Assert.IsTrue(fs.MatchBlank);
        }
```

### See Also

* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


