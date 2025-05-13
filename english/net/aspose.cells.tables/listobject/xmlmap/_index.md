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
public void ListObject_Property_XmlMap()
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

* class [XmlMap](../../../aspose.cells/xmlmap/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


