##Class WorkbookMetadata
Aspose.Cells.Metadata.WorkbookMetadata class. Represents the meta data
## WorkbookMetadata class
Represents the meta data.
```csharp
public class WorkbookMetadata
```
## Constructors
| Name | Description |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Create the meta data object. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Create the meta data object. |
## Properties
| Name | Description |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Returns a [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Gets the options of the metadata. |
## Methods
| Name | Description |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Save the modified metadata to the stream. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Save the modified metadata to the file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metadata;
using Aspose.Cells.Properties;
using System;
using System.IO;
public class WorkbookMetadataDemo
{
public static void WorkbookMetadataExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)
