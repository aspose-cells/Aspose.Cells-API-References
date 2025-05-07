---
title: XmlDataBinding.Url
second_title: Aspose.Cells for .NET API Reference
description: XmlDataBinding property. Gets source url of this data binding
type: docs
url: /net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Gets source url of this data binding.

```csharp
public string Url { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
[Test]
        public void Property_Url()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-46307.xls");
            string url1 = @"D:\For Aspose\XML Tables\Country List.xml";
            string url2 = @"D:\For Aspose\XML Tables\Food List.xml";

            Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
            Assert.AreEqual(url2, wb.Worksheets[1].ListObjects[0].XmlMap.DataBinding.Url);

            wb.Save(Constants.destPath + "CELLSNET-46307.xls");
        }
```

### See Also

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


