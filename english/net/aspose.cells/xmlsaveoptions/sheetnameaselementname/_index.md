---
title: XmlSaveOptions.SheetNameAsElementName
second_title: Aspose.Cells for .NET API Reference
description: XmlSaveOptions property. Indicates whether exporting sheets name as the name of the element
type: docs
url: /net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Indicates whether exporting sheet's name as the name of the element.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Examples

```csharp
// Called: saveOptions.SheetNameAsElementName = false;
public void XmlSaveOptions_Property_SheetNameAsElementName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    XmlSaveOptions saveOptions = new XmlSaveOptions();
    saveOptions.SheetNameAsElementName = false;
    workbook.Save(Constants.destPath + "example.xml", saveOptions);
    XmlLoadOptions loadOptions = new XmlLoadOptions();
    loadOptions.ContainsMultipleWorksheets = true;
    workbook = new Workbook(Constants.destPath + "example.xml", loadOptions);
    workbook.Save(Constants.destPath + "example.xlsx");
    Assert.AreEqual("Firstname", workbook.Worksheets[0].Cells["C3"].StringValue);
            
}
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


