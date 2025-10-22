##ContentTypeProperty.Type
ContentTypeProperty property. Gets and sets the type of the property
## ContentTypeProperty.Type property
Gets and sets the type of the property.
```csharp
public string Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class ContentTypePropertyPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add content type properties with different types
workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
workbook.ContentTypeProperties.Add("Version", "1.0", "number");
workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");
// Access and display property types
foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
{
Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
}
// Save the workbook
workbook.Save("ContentTypePropertyDemo.xlsx");
}
}
}
```
### See Also
* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
