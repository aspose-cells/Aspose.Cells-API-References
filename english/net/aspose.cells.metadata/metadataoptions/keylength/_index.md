---
title: MetadataOptions.KeyLength
second_title: Aspose.Cells for .NET API Reference
description: MetadataOptions property. The key length
type: docs
url: /net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

The key length.

```csharp
public int KeyLength { get; set; }
```

### Examples

```csharp
// Called: options.KeyLength = 256;
public static void Property_KeyLength()
        {
            // Create an instance of MetadataOptions with a specific MetadataType
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Set properties
            options.Password = &quot;your_password&quot;;
            options.KeyLength = 256;

            // Load metadata from an existing workbook
            WorkbookMetadata metadata = new WorkbookMetadata(&quot;MetadataOptionsExample_original.xlsx&quot;, options);

            // Add a custom document property
            metadata.CustomDocumentProperties.Add(&quot;Author&quot;, &quot;John Doe&quot;);

            // Save the metadata changes to a new file
            metadata.Save(&quot;MetadataOptionsExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


