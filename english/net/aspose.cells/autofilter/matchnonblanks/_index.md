---
title: AutoFilter.MatchNonBlanks
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Match all not blank cell in the list
type: docs
url: /net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Match all not blank cell in the list.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Examples

```csharp
// Called: filter.MatchNonBlanks(1);
[Test]
     public void Method_Int32_()
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

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


