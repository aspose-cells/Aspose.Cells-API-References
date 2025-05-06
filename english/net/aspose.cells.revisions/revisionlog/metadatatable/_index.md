---
title: RevisionLog.MetadataTable
second_title: Aspose.Cells for .NET API Reference
description: RevisionLog property. Gets table that contains metadata about a list of specific changes that have taken place for this workbook
type: docs
url: /net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Gets table that contains metadata about a list of specific changes that have taken place for this workbook.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Simon Zhao&amp;quot;, workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
[Test]
        public void Property_MetadataTable()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cellsnet52429.xls&quot;);
           Assert.AreEqual(&quot;Simon Zhao&quot;, workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
        }
```

### See Also

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


