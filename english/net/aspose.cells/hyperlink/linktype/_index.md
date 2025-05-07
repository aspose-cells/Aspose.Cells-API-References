---
title: Hyperlink.LinkType
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Gets the link type
type: docs
url: /net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Gets the link type.

```csharp
public TargetModeType LinkType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(TargetModeType.External, links[0].LinkType);
[Test]
        public void Property_LinkType()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("A1");
            Hyperlink[] links = range.Hyperlinks;
            Assert.AreEqual(TargetModeType.External, links[0].LinkType);
            if(links.Length != 0)
            {
                links[0].Delete();
            }
            Assert.AreEqual(0, workbook.Worksheets[0].Hyperlinks.Count); 
        }
```

### See Also

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


