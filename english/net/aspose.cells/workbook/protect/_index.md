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
// Called: wb.Protect(ProtectionType.All, &amp;quot;p1&amp;quot;);
[Test]
        public void Method_String_()
        {
            var wb = new Workbook()
        {
            BuiltInDocumentProperties =
                {
                Category = &quot;category&quot;,
                   ContentStatus = &quot;contentStatus&quot;,
                }
        };

        wb.Protect(ProtectionType.All, &quot;p1&quot;);
            var xlsStream = new MemoryStream();

        wb.Save(xlsStream, SaveFormat.Excel97To2003);
            xlsStream.Position = 0;

            var wb2 = new Workbook(xlsStream);
        var bip = wb.BuiltInDocumentProperties;
            Assert.AreEqual(&quot;category&quot;, bip.Category);
            Assert.AreEqual(&quot;contentStatus&quot;, bip.ContentStatus);

            var bip2 = wb2.BuiltInDocumentProperties;

            Assert.AreEqual(&quot;category&quot;, bip2.Category);
            Assert.AreEqual(&quot;contentStatus&quot;, bip2.ContentStatus);
        }
```

### See Also

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


