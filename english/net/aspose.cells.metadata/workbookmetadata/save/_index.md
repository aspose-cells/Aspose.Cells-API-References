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
// Called: doc.Save(Constants.destPath + &amp;quot;dest.xls&amp;quot;);
[Test]
        public void Method_String_()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + &quot;CellsNet44144.xls&quot;, new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add(&quot;text1&quot;, &quot;text2&quot;);
            doc.CustomDocumentProperties.Add(&quot;num1&quot;, 1);
            doc.Save(Constants.destPath + &quot;dest.xls&quot;);
            Workbook workbook = new Workbook(Constants.destPath + &quot;dest.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;Data&quot;);
            Assert.AreEqual(doc.CustomDocumentProperties[&quot;text1&quot;].Value.ToString(), &quot;text2&quot;);


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


