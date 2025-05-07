---
title: Workbook.Protect
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Protects a workbook
type: docs
url: /net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Protects a workbook.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | ProtectionType | Protection type. |
| password | String | Password to protect the workbook. |

### Examples

```csharp
// Called: wb.Protect(ProtectionType.All, "p1");
[Test]
        public void Method_String_()
        {
            var wb = new Workbook()
        {
            BuiltInDocumentProperties =
                {
                Category = "category",
                   ContentStatus = "contentStatus",
                }
        };

        wb.Protect(ProtectionType.All, "p1");
            var xlsStream = new MemoryStream();

        wb.Save(xlsStream, SaveFormat.Excel97To2003);
            xlsStream.Position = 0;

            var wb2 = new Workbook(xlsStream);
        var bip = wb.BuiltInDocumentProperties;
            Assert.AreEqual("category", bip.Category);
            Assert.AreEqual("contentStatus", bip.ContentStatus);

            var bip2 = wb2.BuiltInDocumentProperties;

            Assert.AreEqual("category", bip2.Category);
            Assert.AreEqual("contentStatus", bip2.ContentStatus);
        }
```

### See Also

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


