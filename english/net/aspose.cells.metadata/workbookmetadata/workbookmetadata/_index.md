---
title: WorkbookMetadata.WorkbookMetadata
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata constructor. Create the meta data object
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Create the meta data object.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |
| options | MetadataOptions |  |

### Examples

```csharp
// Called: WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "CellsNet44144.xlsx", new MetadataOptions(MetadataType.DocumentProperties));
[Test]
        public void WorkbookMetadata_Constructor()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "CellsNet44144.xlsx", new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            doc.Save(Constants.destPath + "dest.xlsx");
            Workbook workbook = new Workbook(Constants.destPath + "dest.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Data");
            Assert.AreEqual(doc.CustomDocumentProperties["text1"].Value.ToString(), "text2");


        }
```

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Create the meta data object.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| options | MetadataOptions |  |

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


