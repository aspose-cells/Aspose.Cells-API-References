---
title: Worksheet.QueryTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets QueryTableCollection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Gets [`QueryTableCollection`](../../querytablecollection/) in the worksheet.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Examples

```csharp
// Called: QueryTable qt = workbook.Worksheets[0].QueryTables[0];
public void Worksheet_Property_QueryTables()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    QueryTable qt = workbook.Worksheets[0].QueryTables[0];
   Assert.AreEqual("A1:A8", qt.ResultRange.Address);
}
```

### See Also

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


