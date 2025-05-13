---
title: BuiltInDocumentPropertyCollection.DocumentVersion
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Represents the version of the file
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

Represents the version of the file.

```csharp
public string DocumentVersion { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("test_version", wb.BuiltInDocumentProperties.DocumentVersion);
public void BuiltInDocumentPropertyCollection_Property_DocumentVersion()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    //Console.WriteLine(wb.BuiltInDocumentProperties.ContentType);
    Assert.AreEqual("test_content_status", wb.BuiltInDocumentProperties.ContentStatus);
    Assert.AreEqual("test_version", wb.BuiltInDocumentProperties.DocumentVersion);
    // wb.Worksheets[0].ListObjects[0].ConvertToRange();
    // wb.Worksheets[1].ListObjects[0].ConvertToRange();
    Util.ReSave(wb, SaveFormat.Xlsx);
    wb = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual("test_content_type", wb.BuiltInDocumentProperties.ContentType);
    Assert.AreEqual("test_content_status", wb.BuiltInDocumentProperties.ContentStatus);
    Assert.AreEqual("test_version", wb.BuiltInDocumentProperties.DocumentVersion);
    // wb.Worksheets[0].ListObjects[0].ConvertToRange();
    // wb.Worksheets[1].ListObjects[0].ConvertToRange();
    Util.ReSave(wb, SaveFormat.Xlsx);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


