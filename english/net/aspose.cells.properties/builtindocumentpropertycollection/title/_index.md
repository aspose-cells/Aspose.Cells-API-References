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
// Called: Console.WriteLine("Litera Metadact Properties Document",workbook.BuiltInDocumentProperties.Title);
[Test]
        public void Property_Title()
        {
            var filePath = Constants.sourcePath + "CellsNet56344.xls";
            var loadOptions = new LoadOptions();
            loadOptions.Password = "test";

            Console.WriteLine(DateTime.Now);
            Workbook workbook = new Workbook(filePath, loadOptions);
            //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Settings.Password = null;
            workbook.Save(Constants.destPath + "CellsNet56344.xlsx");

            workbook = new Workbook(Constants.destPath + "CellsNet56344.xlsx");
            workbook.Settings.Password = "1";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.EncryptDocumentProperties = false;
            workbook.Save(Constants.destPath + "CellsNet56344.xls", saveOptions);

            LoadOptions xlsOptions = new LoadOptions();
            xlsOptions.Password = "1";
            workbook = new Workbook(Constants.destPath + "CellsNet56344.xls", xlsOptions);
            //Litera Metadact Properties Document
            Console.WriteLine("Litera Metadact Properties Document",workbook.BuiltInDocumentProperties.Title);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


