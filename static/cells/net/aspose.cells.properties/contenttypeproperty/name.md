##ContentTypeProperty.Name
ContentTypeProperty property. Returns or sets the name of the object
## ContentTypeProperty.Name property
Returns or sets the name of the object.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ContentTypePropertyPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a content type property with name "ss"
workbook.ContentTypeProperties.Add("ss", "bb", "text");
// Save to XLS format
workbook.Save("example.xls");
// Reload the workbook and verify the Name property
workbook = new Workbook("example.xls");
Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
// Save to XLSX format
workbook.Save("example.xlsx");
// Reload and verify again
workbook = new Workbook("example.xlsx");
Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
}
}
}
```
### See Also
* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
