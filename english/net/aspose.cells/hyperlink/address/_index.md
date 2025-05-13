---
title: Hyperlink.Address
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the address of a hyperlink
type: docs
url: /net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Represents the address of a hyperlink.

```csharp
public string Address { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("http://www.google.com/", links[1].Address);
public void Hyperlink_Property_Address()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    HyperlinkCollection links = workbook.Worksheets[0].Hyperlinks;
    Assert.AreEqual(3,links.Count);
    Assert.AreEqual("http://www.baidu.com/",links[0].Address);
    Assert.AreEqual("http://www.google.com/",links[1].Address);
    Assert.AreEqual("Sheet1!F3",links[2].Address);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.AreEqual(3, links.Count);
    Assert.AreEqual("http://www.baidu.com/", links[0].Address);
    Assert.AreEqual("http://www.google.com/", links[1].Address);
    Assert.AreEqual("Sheet1!F3", links[2].Address);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


