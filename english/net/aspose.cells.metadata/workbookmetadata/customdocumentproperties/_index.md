---
title: WorkbookMetadata.CustomDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata property. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Examples

```csharp
// Called: meta.CustomDocumentProperties.Add("test", "test");
public void WorkbookMetadata_Property_CustomDocumentProperties()
{
    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
    WorkbookMetadata meta = new WorkbookMetadata(Constants.sourcePath + "example.xlsx", options);
    meta.CustomDocumentProperties.Add("test", "test");
    meta.Save(Constants.destPath + "example.xlsx");
    Workbook w = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual("test", w.CustomDocumentProperties["test"].Value);
}
```

### See Also

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


