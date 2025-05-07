---
title: Worksheet.UniqueId
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets the unique id it is same as 15DB5C3CA5A148AF8F253D86AC232D4F
type: docs
url: /net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("{00000000-0001-0000-0100-000000000000}", workbook.Worksheets[1].UniqueId);
[Test]
        public void Property_UniqueId()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJAVA45271.xlsx");
            Assert.AreEqual("{00000000-0001-0000-0000-000000000000}", workbook.Worksheets[0].UniqueId);
            Assert.AreEqual("{00000000-0001-0000-0100-000000000000}", workbook.Worksheets[1].UniqueId);
            Assert.AreEqual("{00000000-0001-0000-0200-000000000000}", workbook.Worksheets[2].UniqueId);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


