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
// Called: findoptions.SearchOrderByRows = false; ;
private void Property_SearchOrderByRows(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            FindOptions findoptions = new FindOptions();
            findoptions.SearchOrderByRows = false; ;
            Cell cell = cells.Find("abc", null, findoptions);
            AssertHelper.AreEqual(3, cell.Row, "cell.Row");
            AssertHelper.AreEqual(0, cell.Column, "cell.Column");
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


