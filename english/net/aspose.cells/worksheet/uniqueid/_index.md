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
// Called: Assert.AreEqual(id, workbook.Worksheets[0].UniqueId);
[Test]
        public void Property_UniqueId()
        {
            string id = &quot;{&quot; + Guid.NewGuid().ToString() + &quot;}&quot;;
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].UniqueId = id;
            workbook.Save(Constants.destPath + &quot;SheetUniqueId.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;SheetUniqueId.xlsx&quot;);
            Assert.AreEqual(id, workbook.Worksheets[0].UniqueId);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


