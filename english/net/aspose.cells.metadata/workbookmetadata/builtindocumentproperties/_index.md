---
title: WorkbookMetadata.BuiltInDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata property. Returns a DocumentProperty collection that represents all the builtin document properties of the spreadsheet
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Examples

```csharp
// Called: BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;
public static void Property_BuiltInDocumentProperties()
        {
            // Define the file path
            string filePath = &quot;MetadataTypeExample_original.xlsx&quot;;

            // Create MetadataOptions for DocumentProperties
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Load the workbook metadata
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Access built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Access custom document properties
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Display some built-in properties
            Console.WriteLine(&quot;Title: &quot; + builtInProperties[&quot;Title&quot;]);
            Console.WriteLine(&quot;Author: &quot; + builtInProperties[&quot;Author&quot;]);
            Console.WriteLine(&quot;Company: &quot; + builtInProperties[&quot;Company&quot;]);

            // Add a custom property
            customProperties.Add(&quot;MyCustomProperty&quot;, &quot;CustomValue&quot;);

            // save to a different file
            string newFilePath = &quot;MetadataTypeExample.xlsx&quot;;
            metadata.Save(newFilePath);

            Console.WriteLine(&quot;Metadata updated and saved successfully.&quot;);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


