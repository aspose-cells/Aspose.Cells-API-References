##DocumentProperty.Name
DocumentProperty property. Returns the name of the property
## DocumentProperty.Name property
Returns the name of the property.
```csharp
public string Name { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access document properties
BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
// Add a custom property and demonstrate Name usage
DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
Console.WriteLine("Property Name: " + authorProperty.Name);
Console.WriteLine("Property Value: " + authorProperty.Value);
// Access a built-in property by name
DocumentProperty titleProperty = builtInProps["Title"];
titleProperty.Value = "Sample Document";
Console.WriteLine("Title Property Name: " + titleProperty.Name);
Console.WriteLine("Title Property Value: " + titleProperty.Value);
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
