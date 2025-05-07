---
title: RevisionHeader.UserName
second_title: Aspose.Cells for .NET API Reference
description: RevisionHeader property. Gets and sets the name of the user making the revision
type: docs
url: /net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Gets and sets the name of the user making the revision.

```csharp
public string UserName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Simon Zhao", workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
[Test]
        public void Property_UserName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Cellsnet52429.xls");
           Assert.AreEqual("Simon Zhao", workbook.Worksheets.RevisionLogs[0].MetadataTable.UserName);
        }
```

### See Also

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


