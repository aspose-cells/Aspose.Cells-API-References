---
title: SaveOptions.EncryptDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether encrypt document properties when saving as .xls file. The default value is true
type: docs
url: /net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Remarks

Only for .xls,xlsx,xlsb and xlsm file.

### Examples

```csharp
// Called: saveOptions.EncryptDocumentProperties = false;
public void SaveOptions_Property_EncryptDocumentProperties()
{
    var filePath = Constants.sourcePath + "example.xls";
    var loadOptions = new LoadOptions();
    loadOptions.Password = "test";

    Console.WriteLine(DateTime.Now);
    Workbook workbook = new Workbook(filePath, loadOptions);
    //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
    workbook.Settings.Password = null;
    workbook.Save(Constants.destPath + "example.xlsx");

    workbook = new Workbook(Constants.destPath + "example.xlsx");
    workbook.Settings.Password = "1";
    XlsSaveOptions saveOptions = new XlsSaveOptions();
    saveOptions.EncryptDocumentProperties = false;
    workbook.Save(Constants.destPath + "example.xls", saveOptions);

    LoadOptions xlsOptions = new LoadOptions();
    xlsOptions.Password = "1";
    workbook = new Workbook(Constants.destPath + "example.xls", xlsOptions);
    //Litera Metadact Properties Document
    Console.WriteLine("Litera Metadact Properties Document",workbook.BuiltInDocumentProperties.Title);
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


