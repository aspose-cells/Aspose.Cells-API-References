---
title: Workbook.HasRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets if the workbook has any tracked changes
type: docs
url: /net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Gets if the workbook has any tracked changes

```csharp
public bool HasRevisions { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.HasRevisions);
[Test]
        public void Property_HasRevisions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet51116.xls");
            Assert.IsFalse(workbook.HasRevisions);
            workbook.Save(Constants.destPath + "CellsNet51116.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet51116.xls");
            Assert.IsFalse(workbook.HasRevisions);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


