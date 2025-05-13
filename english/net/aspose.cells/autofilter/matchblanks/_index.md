---
title: AutoFilter.MatchBlanks
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Match all blank cell in the list
type: docs
url: /net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Match all blank cell in the list.

```csharp
public void MatchBlanks(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Examples

```csharp
// Called: filter.MatchBlanks(2);
public void AutoFilter_Method_MatchBlanks()
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

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


