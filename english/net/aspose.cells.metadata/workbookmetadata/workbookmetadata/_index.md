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
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodCtorWithStringMetadataOptionsDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xls";
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);
            
            Console.WriteLine("WorkbookMetadata created successfully with document properties metadata.");
        }
    }
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

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;
    using System.IO;

    public class WorkbookMetadataConstructorWithStreamMetadataOptionsDemo
    {
        public static void Run()
        {
            // Create a temporary file stream for demonstration
            MemoryStream stream = new MemoryStream();
            using (Workbook tempWorkbook = new Workbook())
            {
                tempWorkbook.Save(stream, SaveFormat.Xlsx);
            }
            stream.Position = 0;

            // Create MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            try
            {
                // Call the #ctor method with Stream and MetadataOptions parameters
                WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                // Display metadata information
                Console.WriteLine("WorkbookMetadata created successfully with Stream and MetadataOptions");
                Console.WriteLine($"Metadata Options Type: {metadata.Options.MetadataType}");
                Console.WriteLine($"Built-in Properties Count: {metadata.BuiltInDocumentProperties.Count}");
                Console.WriteLine($"Custom Properties Count: {metadata.CustomDocumentProperties.Count}");

                // Save the metadata to a new file
                metadata.Save("WorkbookMetadataWithStream.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating WorkbookMetadata: {ex.Message}");
            }
            finally
            {
                stream.Dispose();
            }
        }
    }
}
```

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


