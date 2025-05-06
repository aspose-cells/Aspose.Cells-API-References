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
// Called: WorkbookMetadata meta = new WorkbookMetadata(&amp;quot;WorkbookMetadataExample_original.xlsx&amp;quot;, options);
public static void WorkbookMetadata_Constructor()
        {
            // Create MetadataOptions instance
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Create WorkbookMetadata instance with a file name and options
            WorkbookMetadata meta = new WorkbookMetadata(&quot;WorkbookMetadataExample_original.xlsx&quot;, options);

            // Add a custom document property
            meta.CustomDocumentProperties.Add(&quot;test&quot;, &quot;test&quot;);

            // Save the metadata to a new file
            meta.Save(&quot;WorkbookMetadataExample.xlsx&quot;);

            // Demonstrate accessing built-in document properties
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine(&quot;Author: &quot; + builtInProps.Author);
            Console.WriteLine(&quot;Title: &quot; + builtInProps.Title);

            // Demonstrate accessing custom document properties
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine(&quot;Custom Property - Name: &quot; + prop.Name + &quot;, Value: &quot; + prop.Value);
            }

            // Save the metadata to a stream
            using (FileStream stream = new FileStream(&quot;WorkbookMetadataExample2.xlsx&quot;, FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
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

### See Also

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


