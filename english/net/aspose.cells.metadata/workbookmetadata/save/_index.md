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

### Examples

```csharp
namespace AsposeCellsExamples.WorkbookMetadataMethodSaveWithStreamDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;
    using System.IO;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            // Create a temporary file to work with
            string tempFile = Path.GetTempFileName();
            try
            {
                // Create a new workbook and save it to the temp file
                Workbook workbook = new Workbook();
                workbook.Save(tempFile);

                // Create metadata options
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Create WorkbookMetadata instance
                WorkbookMetadata metadata = new WorkbookMetadata(tempFile, options);

                // Add some document properties
                metadata.BuiltInDocumentProperties.Author = "Test Author";
                metadata.BuiltInDocumentProperties.Title = "Test Title";
                metadata.CustomDocumentProperties.Add("CustomProperty", "Custom Value");

                // Create a memory stream to save the metadata
                using (MemoryStream stream = new MemoryStream())
                {
                    try
                    {
                        // Call the Save method with Stream parameter
                        metadata.Save(stream);

                        Console.WriteLine("Metadata saved to stream successfully");
                        Console.WriteLine($"Stream length: {stream.Length} bytes");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error saving metadata to stream: {ex.Message}");
                    }
                }
            }
            finally
            {
                // Clean up the temporary file
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### See Also

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


