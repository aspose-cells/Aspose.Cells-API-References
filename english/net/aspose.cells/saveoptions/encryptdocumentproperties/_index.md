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
            var filePath = Constants.sourcePath + &quot;CellsNet56344.xls&quot;;
            var loadOptions = new LoadOptions();
            loadOptions.Password = &quot;test&quot;;

            Console.WriteLine(DateTime.Now);
            Workbook workbook = new Workbook(filePath, loadOptions);
            //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Settings.Password = null;
            workbook.Save(Constants.destPath + &quot;CellsNet56344.xlsx&quot;);

            workbook = new Workbook(Constants.destPath + &quot;CellsNet56344.xlsx&quot;);
            workbook.Settings.Password = &quot;1&quot;;
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.EncryptDocumentProperties = false;
            workbook.Save(Constants.destPath + &quot;CellsNet56344.xls&quot;, saveOptions);

            LoadOptions xlsOptions = new LoadOptions();
            xlsOptions.Password = &quot;1&quot;;
            workbook = new Workbook(Constants.destPath + &quot;CellsNet56344.xls&quot;, xlsOptions);
            //Litera Metadact Properties Document
            Console.WriteLine(&quot;Litera Metadact Properties Document&quot;,workbook.BuiltInDocumentProperties.Title);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


