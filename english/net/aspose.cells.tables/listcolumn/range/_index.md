---
title: ListColumn.Range
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets the range of this list column
type: docs
url: /net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Gets the range of this list column.

```csharp
public Range Range { get; }
```

### Examples

```csharp
// Called: Aspose.Cells.Range rang = listC.Range;
public void ListColumn_Property_Range()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ListColumn listC = workbook.Worksheets[0].ListObjects[0].ListColumns[0];
    Aspose.Cells.Range rang = listC.Range;
    Assert.AreEqual(12, rang.RowCount);

}
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


