---
title: XmlSaveOptions.XmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XmlSaveOptions constructor. Creates options for saving xml file
type: docs
url: /net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Creates options for saving xml file.

```csharp
public XmlSaveOptions()
```

### Examples

```csharp
// Called: saveOptions = new XmlSaveOptions();
public void XmlSaveOptions_Constructor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    XmlSaveOptions saveOptions = new XmlSaveOptions();
    saveOptions.SheetNameAsElementName = true;
    workbook.Save(Constants.destPath + "example.xml", saveOptions);
    string text = File.ReadAllText(Constants.destPath + "example.xml");
    Assert.IsTrue(text.IndexOf("<c>63</c>") != -1);

    saveOptions = new XmlSaveOptions();
    saveOptions.SheetNameAsElementName = true;
    saveOptions.DataAsAttribute = true;
    workbook.Save(Constants.destPath + "example.xml", saveOptions);
    text = File.ReadAllText(Constants.destPath + "example.xml");

    Assert.IsTrue(text.IndexOf("c=\"63\"") != -1);

}
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


