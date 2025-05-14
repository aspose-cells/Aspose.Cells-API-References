---
title: RevisionLogCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: RevisionLogCollection property. Gets RevisionLog by index
type: docs
url: /net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Gets [`RevisionLog`](../../revisionlog/) by index.

```csharp
public RevisionLog this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

Returns [`RevisionLog`](../../revisionlog/) object.

### Examples

```csharp
// Called: Assert.AreEqual("Simon Zhao", workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
public void RevisionLogCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
   Assert.AreEqual("Simon Zhao", workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
}
```

### See Also

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


