##CustomDocumentPropertyCollection.Add
CustomDocumentPropertyCollection method. Creates a new custom document property of the PropertyType.String data type
## Add(string, string) {#add_4}
Creates a new custom document property of the **PropertyType.String** data type.
```csharp
public DocumentProperty Add(string name, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | String | The value of the property. |
### Return Value
The newly created property object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomDocumentPropertyCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.CustomDocumentProperties.Add("startdate", "ToneyTest");
Console.WriteLine("Custom Property Value: " +
workbook.CustomDocumentProperties["startdate"].Value);
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## Add(string, int) {#add_2}
Creates a new custom document property of the **PropertyType.Number** data type.
```csharp
public DocumentProperty Add(string name, int value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Int32 | The value of the property. |
### Return Value
The newly created property object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomDocumentPropertyCollectionMethodAddWithStringInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet1");
// Add custom document properties
workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
workbook.CustomDocumentProperties.Add("numericProperty", 42);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the properties
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## Add(string, DateTime) {#add_3}
Creates a new custom document property of the **PropertyType.DateTime** data type.
```csharp
public DocumentProperty Add(string name, DateTime value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | DateTime | The value of the property. |
### Return Value
The newly created property object.
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## Add(string, bool) {#add}
Creates a new custom document property of the **PropertyType.Boolean** data type.
```csharp
public DocumentProperty Add(string name, bool value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Boolean | The value of the property. |
### Return Value
The newly created property object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class CustomDocumentPropertyCollectionMethodAddWithStringBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;
// Add boolean custom property
customProperties.Add("IsApproved", true);
// Display the added property
DocumentProperty property = customProperties["IsApproved"];
Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
// Save the workbook
workbook.Save("CustomPropertiesExample.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## Add(string, double) {#add_1}
Creates a new custom document property of the **PropertyType.Float** data type.
```csharp
public DocumentProperty Add(string name, double value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Double | The value of the property. |
### Return Value
The newly created property object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class CustomDocumentPropertyCollectionMethodAddWithStringDoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Demonstrate Add method with String and Double parameters
customProperties.Add("Rating", 4.5);
customProperties.Add("Score", 8.75);
// Access and display the added properties
DocumentProperty ratingProperty = customProperties["Rating"];
DocumentProperty scoreProperty = customProperties["Score"];
Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
Console.WriteLine($"Score: {scoreProperty.ToDouble()}");
workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
