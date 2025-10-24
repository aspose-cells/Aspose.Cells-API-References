##WorkbookMetadata.Save
WorkbookMetadata method. Save the modified metadata to the file
## Save(string) {#save_1}
Save the modified metadata to the file.
```csharp
public void Save(string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;
namespace AsposeCellsExamples
{
public class WorkbookMetadataMethodSaveWithStringDemo
{
public static void Run()
{
// Create a new workbook metadata
WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
// Add custom properties
doc.CustomDocumentProperties.Add("text1", "text2");
doc.CustomDocumentProperties.Add("num1", 1);
// Save with string path
doc.Save("output.xlsb");
// Verify the saved file
Workbook workbook = new Workbook("output.xlsb");
Console.WriteLine("File saved successfully with custom properties.");
Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
}
}
}
```
### See Also
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
## Save(Stream) {#save}
Save the modified metadata to the stream.
```csharp
public void Save(Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
### See Also
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
