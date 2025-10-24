##DocumentProperty.IsGeneratedName
DocumentProperty property. Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API
## DocumentProperty.IsGeneratedName property
Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.
```csharp
public bool IsGeneratedName { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class DocumentPropertyPropertyIsGeneratedNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
// Access custom document properties for adding
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a custom property
DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
// Display IsGeneratedName for built-in property
DocumentProperty authorProperty = properties["Author"];
Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
// Display IsGeneratedName for custom property
Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);
// Create a scenario where a property might have a generated name
// (Note: In practice, IsGeneratedName is read-only and set internally by Aspose.Cells)
DocumentProperty generatedNameProperty = properties["_PID_GUID"];
if (generatedNameProperty != null)
{
Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
}
// Save the workbook
workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
