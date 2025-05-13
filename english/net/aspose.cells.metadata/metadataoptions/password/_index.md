---
title: MetadataOptions.Password
second_title: Aspose.Cells for .NET API Reference
description: MetadataOptions property. Represents Workbook file encryption password
type: docs
url: /net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Represents Workbook file encryption password.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: options.Password = "your_password";
public static void MetadataOptions_Property_Password()
        {
            // Create an instance of MetadataOptions with a specific MetadataType
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Set properties
            options.Password = "your_password";
            options.KeyLength = 256;

            // Load metadata from an existing workbook
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Add a custom document property
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Save the metadata changes to a new file
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
```

### See Also

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


