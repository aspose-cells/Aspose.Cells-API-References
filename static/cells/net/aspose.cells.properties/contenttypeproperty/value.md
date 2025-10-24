##ContentTypeProperty.Value
ContentTypeProperty property. Returns or sets the value of the content type property
## ContentTypeProperty.Value property
Returns or sets the value of the content type property.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class ContentTypePropertyPropertyValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add a content type property
workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
// Access and modify the property's Value
ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
property.Value = "Aspose"; // Demonstrating Value property usage
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
