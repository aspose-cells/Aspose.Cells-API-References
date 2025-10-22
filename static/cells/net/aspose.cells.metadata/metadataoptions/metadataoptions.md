##MetadataOptions.MetadataOptions
MetadataOptions constructor. Creates an options of loading the metadata
## MetadataOptions constructor
Creates an options of loading the metadata.
```csharp
public MetadataOptions(MetadataType metadataType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| metadataType | MetadataType | The type of metadata. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metadata;
using System;
public class MetadataOptionsMethodCtorWithMetadataTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Call the #ctor method with MetadataType parameter
MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
// Set additional properties
options.Password = "test123";
options.KeyLength = 128;
// Display the created options
Console.WriteLine($"MetadataType: {options.MetadataType}");
Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
Console.WriteLine($"KeyLength: {options.KeyLength}");
// Use the options when loading metadata (example)
// This would typically be used with LoadOptions when opening a file
// Note: The original code tried to set MetadataOptions directly on LoadOptions,
// but the LoadOptions class doesn't have this property in the provided definition.
// We'll just keep the options creation part since the usage with LoadOptions
// isn't possible with the current API definition.
Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
}
catch (Exception ex)
{
Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
}
// Save the workbook (though metadata options wouldn't affect this empty workbook)
workbook.Save("MetadataOptionsCtorDemo.xlsx");
}
}
}
```
### See Also
* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
