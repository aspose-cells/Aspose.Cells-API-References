##ContentTypeProperty.IsNillable
ContentTypeProperty property. Indicates whether the value could be empty
## ContentTypeProperty.IsNillable property
Indicates whether the value could be empty.
```csharp
public bool IsNillable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class ContentTypePropertyPropertyIsNillableDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add a content type property
workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
// Access the property and set IsNillable
ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
property.IsNillable = true;
// Verify and output the IsNillable value
Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
}
}
}
```
### See Also
* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
