---
title: BuiltInDocumentPropertyCollection.Title
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the title of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Gets or sets the title of the document.

```csharp
public string Title { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Litera Metadact Properties Document", workbook.BuiltInDocumentProperties.Title);
public void BuiltInDocumentPropertyCollection_Property_Title()
{
    var filePath = Constants.sourcePath + "example.xls";
    var loadOptions = new LoadOptions();
    loadOptions.Password = "test";

    Console.WriteLine(DateTime.Now);
    Workbook workbook = new Workbook(filePath, loadOptions);
    //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
    OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
    saveOptions.EncryptDocumentProperties = false;
    workbook.Save(Constants.destPath + "example.xlsx", saveOptions);
    loadOptions = new LoadOptions();
    loadOptions.Password = "test";
    workbook = new Workbook(Constants.destPath + "example.xlsx", loadOptions);
    Console.WriteLine("Litera Metadact Properties Document", workbook.BuiltInDocumentProperties.Title);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


