---
title: XmlMap.DataBinding
second_title: Aspose.Cells for .NET API Reference
description: XmlMap property. Gets an XmlDataBinding of this map
type: docs
url: /net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Gets an [`XmlDataBinding`](../../xmldatabinding/) of this map.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
public void XmlMap_Property_DataBinding()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
    string url1 = @"D:\For Aspose\XML Tables\Country List.xml";
    string url2 = @"D:\For Aspose\XML Tables\Food List.xml";

    Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
    Assert.AreEqual(url2, wb.Worksheets[1].ListObjects[0].XmlMap.DataBinding.Url);

    wb.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


