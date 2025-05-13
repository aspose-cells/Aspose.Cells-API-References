---
title: Range.Hyperlinks
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets all hyperlink in the range
type: docs
url: /net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Gets all hyperlink in the range.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Examples

```csharp
// Called: Hyperlink[] links = range.Hyperlinks;
public void Range_Property_Hyperlinks()
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

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


