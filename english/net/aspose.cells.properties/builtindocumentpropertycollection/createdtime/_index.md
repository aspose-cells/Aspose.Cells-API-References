---
title: BuiltInDocumentPropertyCollection.CreatedTime
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets date of the document creation in local timezone
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Gets or sets date of the document creation in local timezone.

```csharp
public DateTime CreatedTime { get; set; }
```

### Remarks

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(1, 5, 5);
[Test]
        public void Property_CreatedTime()
        {
            Workbook workbook = new Workbook();
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(1, 5, 5);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.MinValue;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.MinValue;
            Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


