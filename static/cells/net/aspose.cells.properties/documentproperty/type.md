##DocumentProperty.Type
DocumentProperty property. Gets the data type of the property
## DocumentProperty.Type property
Gets the data type of the property.
```csharp
public PropertyType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access custom document properties (not built-in)
CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
// Add custom properties with different types
properties.Add("Author", "John Doe");
properties.Add("CreatedDate", DateTime.Now);
properties.Add("Revision", 5);
properties.Add("IsApproved", true);
// Demonstrate Type property usage
Console.WriteLine("Document Properties and Their Types:");
foreach (DocumentProperty prop in properties)
{
Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
}
// Access specific property and check its type
DocumentProperty dateProp = properties["CreatedDate"];
if (dateProp.Type == PropertyType.DateTime)
{
Console.WriteLine("\nCreatedDate is a DateTime property");
Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
}
}
}
}
```
### See Also
* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
