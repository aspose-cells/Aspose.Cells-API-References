---
title: Cell.IsMerged
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks if a cell is part of a merged range or not
type: docs
url: /net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Checks if a cell is part of a merged range or not.

```csharp
public bool IsMerged { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["N3"].IsMerged);
[Test]
        public void Property_IsMerged()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSAPP1224.json");
            Assert.AreEqual("ddd", workbook.Worksheets[0].Cells["N3"].StringValue);
            Assert.IsTrue(workbook.Worksheets[0].Cells["N3"].IsMerged);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


