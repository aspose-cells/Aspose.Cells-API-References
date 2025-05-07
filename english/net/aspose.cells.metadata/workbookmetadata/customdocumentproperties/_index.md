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
// Called: doc.CustomDocumentProperties.Add("text1", "text2");
[Test]
        public void Property_CustomDocumentProperties()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "CellsNet44144.xls", new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            doc.Save(Constants.destPath + "dest.xls");
            Workbook workbook = new Workbook(Constants.destPath + "dest.xls");
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Data");
            Assert.AreEqual(doc.CustomDocumentProperties["text1"].Value.ToString(), "text2");


        }
```

### See Also

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


