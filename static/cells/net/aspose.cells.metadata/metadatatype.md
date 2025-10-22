##Enum MetadataType
Aspose.Cells.Metadata.MetadataType enum. Represents the type of metadata
## MetadataType enumeration
Represents the type of metadata.
```csharp
[Flags]
public enum MetadataType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Encryption | `1` | Encrypts the file. |
| Decryption | `2` | Decrypts the file. |
| DocumentProperties | `4` | Load the properties of the file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.Metadata;
using Aspose.Cells.Properties;
using System;
using System.IO;
public class MetadataTypeDemo
{
public static void MetadataTypeExample()
{
// Define the file path
string filePath = "MetadataTypeExample_original.xlsx";
// Create MetadataOptions for DocumentProperties
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
// Load the workbook metadata
WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
// Access built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;
// Access custom document properties
CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;
// Display some built-in properties
Console.WriteLine("Title: " + builtInProperties["Title"]);
Console.WriteLine("Author: " + builtInProperties["Author"]);
Console.WriteLine("Company: " + builtInProperties["Company"]);
// Add a custom property
customProperties.Add("MyCustomProperty", "CustomValue");
// save to a different file
string newFilePath = "MetadataTypeExample.xlsx";
metadata.Save(newFilePath);
Console.WriteLine("Metadata updated and saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)
