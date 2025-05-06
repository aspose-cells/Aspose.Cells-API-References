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
// Called: Assert.AreEqual(doc.CustomDocumentProperties[&amp;quot;text1&amp;quot;].Value.ToString(), &amp;quot;text2&amp;quot;);
[Test]
        public void Property_CustomDocumentProperties()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + &quot;CellsNet44144.xlsb&quot;, new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add(&quot;text1&quot;, &quot;text2&quot;);
            doc.CustomDocumentProperties.Add(&quot;num1&quot;, 1);
            doc.Save(Constants.destPath + &quot;dest.xlsb&quot;);
            Workbook workbook = new Workbook(Constants.destPath + &quot;dest.xlsb&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;Data&quot;);
            Assert.AreEqual(doc.CustomDocumentProperties[&quot;text1&quot;].Value.ToString(), &quot;text2&quot;);


        }
```

### See Also

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


