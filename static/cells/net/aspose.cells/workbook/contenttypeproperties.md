##Workbook.ContentTypeProperties
Workbook property. Gets the list of ContentTypeProperty objects in the workbook
## Workbook.ContentTypeProperties property
Gets the list of [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) objects in the workbook.
```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyContentTypePropertiesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add simple string property
int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
workbook.ContentTypeProperties[index1].IsNillable = true;
// Add datetime property with type specification
int index2 = workbook.ContentTypeProperties.Add("Property2",
DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
workbook.ContentTypeProperties[index2].IsNillable = false;
// Save the workbook
workbook.Save("ContentTypePropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
