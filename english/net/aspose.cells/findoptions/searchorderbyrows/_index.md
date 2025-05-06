---
title: FindOptions.SearchOrderByRows
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates whether search order by rows or columns
type: docs
url: /net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Indicates whether search order by rows or columns.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Examples

```csharp
// Called: findoptions.SearchOrderByRows = true;                ;
private void Property_SearchOrderByRows(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            FindOptions findoptions = new FindOptions();
            findoptions.SearchOrderByRows = true;                ;
            Cell cell = cells.Find(&quot;abc&quot;, null, findoptions);
            AssertHelper.AreEqual(2, cell.Row, &quot;cell.Row&quot;);
            AssertHelper.AreEqual(3, cell.Column, &quot;cell.Column&quot;);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


