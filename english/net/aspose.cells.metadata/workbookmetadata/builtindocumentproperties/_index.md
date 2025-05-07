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
// Called: BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
public static void Property_BuiltInDocumentProperties()
        {
            // Create MetadataOptions instance
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Create WorkbookMetadata instance with a file name and options
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Add a custom document property
            meta.CustomDocumentProperties.Add("test", "test");

            // Save the metadata to a new file
            meta.Save("WorkbookMetadataExample.xlsx");

            // Demonstrate accessing built-in document properties
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Demonstrate accessing custom document properties
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Save the metadata to a stream
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


