---
title: BuiltInDocumentPropertyCollection.CreatedUniversalTime
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the Universal time of the document creation
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/createduniversaltime/
---
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property

Gets or sets the Universal time of the document creation.

```csharp
public DateTime CreatedUniversalTime { get; set; }
```

### Remarks

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: Assert.AreEqual(15, wk.BuiltInDocumentProperties.CreatedUniversalTime.Hour);
[Test]
        public void Property_CreatedUniversalTime()
        {
            Workbook wk = new Workbook(Constants.sourcePath + "CellsNet46342.xlsm");
            Assert.AreEqual(15, wk.BuiltInDocumentProperties.CreatedUniversalTime.Hour);
            wk = Util.ReSave(wk, SaveFormat.Excel97To2003);
            Assert.AreEqual(15, wk.BuiltInDocumentProperties.CreatedUniversalTime.Hour);
            wk = Util.ReSave(wk, SaveFormat.SpreadsheetML);
            Assert.AreEqual(15, wk.BuiltInDocumentProperties.CreatedUniversalTime.Hour);
            wk = Util.ReSave(wk, SaveFormat.Xlsx);
            Assert.AreEqual(15, wk.BuiltInDocumentProperties.CreatedUniversalTime.Hour);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


