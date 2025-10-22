##WorkbookMetadata.Options
WorkbookMetadata property. Gets the options of the metadata
## WorkbookMetadata.Options property
Gets the options of the metadata.
```csharp
public MetadataOptions Options { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metadata;
using System;
public class WorkbookMetadataPropertyOptionsDemo
{
public static void Run()
{
// Create metadata options for document properties
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
options.Password = "test123";
options.KeyLength = 128;
// Create a new workbook metadata instance with options
WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
// Display current options values
Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
Console.WriteLine("Password: " + metadata.Options.Password);
Console.WriteLine("Key Length: " + metadata.Options.KeyLength);
// Access built-in document properties
var builtInProps = metadata.BuiltInDocumentProperties;
builtInProps.Author = "Aspose Developer";
builtInProps.Title = "Metadata Demo";
// Add custom document properties
var customProps = metadata.CustomDocumentProperties;
customProps.Add("Department", "Development");
customProps.Add("Project", "Metadata API");
// Save the metadata changes
metadata.Save("output.xlsx");
// Create new options for encryption
MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
newOptions.Password = "newpassword";
newOptions.KeyLength = 256;
WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
encryptedMetadata.Save("encrypted_output.xlsx");
}
}
}
```
### See Also
* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
