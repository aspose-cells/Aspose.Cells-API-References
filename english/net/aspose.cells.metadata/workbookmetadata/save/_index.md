---
title: WorkbookMetadata.Save
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata method. Save the modified metadata to the file
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Save the modified metadata to the file.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |

### Examples

```csharp
// Called: doc.Save(Constants.destPath + "dest.xlsb");
public void WorkbookMetadata_Method_Save()
{
    WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "example.xlsb", new MetadataOptions(MetadataType.DocumentProperties));
    doc.CustomDocumentProperties.Add("text1", "text2");
    doc.CustomDocumentProperties.Add("num1", 1);
    doc.Save(Constants.destPath + "dest.xlsb");
    Workbook workbook = new Workbook(Constants.destPath + "dest.xlsb");
    Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Data");
    Assert.AreEqual(doc.CustomDocumentProperties["text1"].Value.ToString(), "text2");


}
```

### See Also

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Save the modified metadata to the stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |

### See Also

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


