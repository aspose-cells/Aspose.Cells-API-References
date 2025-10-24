##DocumentProperty.Source
DocumentProperty property. The linked content source
## DocumentProperty.Source property
The linked content source.
```csharp
public string Source { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyPropertySourceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access custom document properties
var properties = workbook.Worksheets.CustomDocumentProperties;
// Add properties
properties.Add("Author", "John Doe");
properties.Add("CreatedDate", DateTime.Now);
properties.Add("Revision", 1);
// Get properties and display their sources
Console.WriteLine("Property Sources:");
Console.WriteLine($"Author: {properties["Author"].Source}");
Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
Console.WriteLine($"Revision: {properties["Revision"].Source}");
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
