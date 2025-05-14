---
title: Worksheet.ListObjects
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all ListObjects in this worksheet
type: docs
url: /net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Gets all ListObjects in this worksheet.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Examples

```csharp
// Called: table = worksheets["S.19.01.01.paid"].ListObjects["ClaimsStored"];
public void Worksheet_Property_ListObjects()
{
    Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    WorksheetCollection worksheets = workbook.Worksheets;
    ListObject table;

    table = worksheets["S.19.01.01.paid"].ListObjects["ClaimsStored"];
    table.Resize(table.StartRow, table.StartColumn, table.EndRow + 17, table.EndColumn, table.ShowHeaderRow);
    table = worksheets["S.19.01.01.RBNS"].ListObjects["ClaimsStored8"];
    table.Resize(table.StartRow, table.StartColumn, table.EndRow + 17, table.EndColumn, table.ShowHeaderRow);
    Assert.AreEqual(worksheets["S.19.01.01.paid"].Cells["J37"].Formula, "=[@C0170]");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


