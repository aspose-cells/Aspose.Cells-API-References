---
title: XmlLoadOptions.IgnoreRootAttributes
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Indicates whether ignore attributes of the root element
type: docs
url: /net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Indicates whether ignore attributes of the root element.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Examples

```csharp
// Called: options.IgnoreRootAttributes = true;
public void XmlLoadOptions_Property_IgnoreRootAttributes()
{
    XmlLoadOptions options = new XmlLoadOptions();
    options.IgnoreRootAttributes = true;
    Workbook lc_WorkBook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xml", options);
    Assert.AreEqual("Capital subscris varsat", lc_WorkBook.Worksheets[0].Cells["AH8"].StringValue);
    lc_WorkBook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


