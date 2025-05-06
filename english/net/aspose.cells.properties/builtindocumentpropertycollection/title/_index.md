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
// Called: Console.WriteLine(&amp;quot;Litera Metadact Properties Document&amp;quot;, workbook.BuiltInDocumentProperties.Title);
[Test]
        public void Property_Title()
        {
            var filePath = Constants.sourcePath + &quot;CellsNet56344.xls&quot;;
            var loadOptions = new LoadOptions();
            loadOptions.Password = &quot;test&quot;;

            Console.WriteLine(DateTime.Now);
            Workbook workbook = new Workbook(filePath, loadOptions);
            //Console.WriteLine(workbook.Settings.WriteProtection.IsWriteProtected);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EncryptDocumentProperties = false;
            workbook.Save(Constants.destPath + &quot;CellsNet56354.xlsx&quot;, saveOptions);
            loadOptions = new LoadOptions();
            loadOptions.Password = &quot;test&quot;;
            workbook = new Workbook(Constants.destPath + &quot;CellsNet56354.xlsx&quot;, loadOptions);
            Console.WriteLine(&quot;Litera Metadact Properties Document&quot;, workbook.BuiltInDocumentProperties.Title);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


