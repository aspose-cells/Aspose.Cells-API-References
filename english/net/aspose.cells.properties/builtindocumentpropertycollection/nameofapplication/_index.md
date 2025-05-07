---
title: BuiltInDocumentPropertyCollection.NameOfApplication
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the name of the application
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Gets or sets the name of the application.

```csharp
public string NameOfApplication { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Microsoft Excel", workbook.BuiltInDocumentProperties.NameOfApplication);
[Test]
        public void Property_NameOfApplication()
        {
            Workbook workbook = new Workbook();
            workbook.Save(Constants.destPath + "CellsJava43438.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsJava43438.xlsx");
            Assert.AreEqual("Microsoft Excel", workbook.BuiltInDocumentProperties.NameOfApplication);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


