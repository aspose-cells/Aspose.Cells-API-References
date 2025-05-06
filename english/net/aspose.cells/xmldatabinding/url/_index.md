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
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-46301.xlsx&quot;);
            string url1 = @&quot;D:\For Aspose\XML Tables\Country List.xml&quot;;
            string url2 = @&quot;D:\For Aspose\XML Tables\Food List.xml&quot;;

            Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
            Assert.AreEqual(url2, wb.Worksheets[1].ListObjects[0].XmlMap.DataBinding.Url);

            wb.Save(Constants.destPath + &quot;CELLSNET-46301.xls&quot;);

        }
```

### See Also

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


