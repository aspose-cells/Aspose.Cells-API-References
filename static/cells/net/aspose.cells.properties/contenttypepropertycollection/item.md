##ContentTypePropertyCollection.Item
ContentTypePropertyCollection property. Gets the content type property by the specific index
## ContentTypePropertyCollection indexer (1 of 2)
Gets the content type property by the specific index.
```csharp
public ContentTypeProperty this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The content type property
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ContentTypePropertyCollectionPropertyItemDemo1
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add content type properties and demonstrate Item property usage
int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
workbook.ContentTypeProperties[index1].IsNillable = true;
int index2 = workbook.ContentTypeProperties.Add("Property2",
DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
workbook.ContentTypeProperties[index2].IsNillable = false;
// Access properties using Item indexer
Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
workbook.Save("ContentTypePropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## ContentTypePropertyCollection indexer (2 of 2)
Gets the content type property by the property name.
```csharp
public ContentTypeProperty this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The property name. |
### Return Value
The content type property
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class ContentTypePropertyCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add content type property
workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
// Access property using Item indexer
ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
// Modify property values
property.Value = "UpdatedValue";
property.IsNillable = false;
// Save workbook
workbook.Save("ContentTypePropertyDemo.xlsx");
}
}
}
```
### See Also
* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
