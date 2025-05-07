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
// Called: saveOptions.SheetNameAsElementName = true;
[Test]
        public void Property_SheetNameAsElementName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet53135.xlsx");
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save(Constants.destPath + "CellsNet53135_1.xml", saveOptions);
            string text = File.ReadAllText(Constants.destPath + "CellsNet53135_1.xml");
            Assert.IsTrue(text.IndexOf("<c>63</c>") != -1);

            saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = true;
            workbook.Save(Constants.destPath + "CellsNet53135_2.xml", saveOptions);
            text = File.ReadAllText(Constants.destPath + "CellsNet53135_2.xml");

            Assert.IsTrue(text.IndexOf("c=\"63\"") != -1);

        }
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


