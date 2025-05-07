---
title: XmlLoadOptions.ContainsMultipleWorksheets
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Indicates whether importing xml as multiple worksheets
type: docs
url: /net/aspose.cells/xmlloadoptions/containsmultipleworksheets/
---
## XmlLoadOptions.ContainsMultipleWorksheets property

Indicates whether importing xml as multiple worksheets.

```csharp
public bool ContainsMultipleWorksheets { get; set; }
```

### Examples

```csharp
// Called: loadOptions.ContainsMultipleWorksheets = true;
[Test]
        public void Property_ContainsMultipleWorksheets()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49717.xlsx");
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save(Constants.destPath + "CELLSNET49717.xml", saveOptions);
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            workbook = new Workbook(Constants.destPath + "CELLSNET49717.xml", loadOptions);
            workbook.Save(Constants.destPath + "CELLSNET49717.xlsx");
            Assert.AreEqual("Firstname", workbook.Worksheets[0].Cells["C3"].StringValue);
            
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


