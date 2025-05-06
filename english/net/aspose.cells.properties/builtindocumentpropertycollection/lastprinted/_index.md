---
title: BuiltInDocumentPropertyCollection.LastPrinted
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the date when the document was last printed in local timezone
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Gets or sets the date when the document was last printed in local timezone.

```csharp
public DateTime LastPrinted { get; set; }
```

### Remarks

If the document was never printed, this property will return DateTime.MinValue.

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: workbook.BuiltInDocumentProperties.LastPrinted = DateTime.MinValue;
[Test]
        public void Property_LastPrinted()
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


