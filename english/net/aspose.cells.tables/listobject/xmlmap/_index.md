---
title: ListObject.XmlMap
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets an XmlMap used for this list
type: docs
url: /net/aspose.cells.tables/listobject/xmlmap/
---
## ListObject.XmlMap property

Gets an `XmlMap` used for this list.

```csharp
public XmlMap XmlMap { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(url2, wb.Worksheets[1].ListObjects[0].XmlMap.DataBinding.Url);
[Test]
        public void Property_XmlMap()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-46307.xls&quot;);
            string url1 = @&quot;D:\For Aspose\XML Tables\Country List.xml&quot;;
            string url2 = @&quot;D:\For Aspose\XML Tables\Food List.xml&quot;;

            Assert.AreEqual(url1, wb.Worksheets[0].ListObjects[0].XmlMap.DataBinding.Url);
            Assert.AreEqual(url2, wb.Worksheets[1].ListObjects[0].XmlMap.DataBinding.Url);

            wb.Save(Constants.destPath + &quot;CELLSNET-46307.xls&quot;);
        }
```

### See Also

* class [XmlMap](../../../aspose.cells/xmlmap/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


