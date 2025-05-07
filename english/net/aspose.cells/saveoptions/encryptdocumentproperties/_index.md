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
[Test]
        public void Property_EncryptDocumentProperties()
        {
            var filePath = Constants.sourcePath + "CellsNet56344.xls";
            var loadOptions = new LoadOptions();
            loadOptions.Password = "test";

            Console.WriteLine(DateTime.Now);
            Workbook workbook = new Workbook(filePath, loadOptions);
            //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EncryptDocumentProperties = false;
            workbook.Save(Constants.destPath + "CellsNet56354.xlsx", saveOptions);
            loadOptions = new LoadOptions();
            loadOptions.Password = "test";
            workbook = new Workbook(Constants.destPath + "CellsNet56354.xlsx", loadOptions);
            Console.WriteLine("Litera Metadact Properties Document", workbook.BuiltInDocumentProperties.Title);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


