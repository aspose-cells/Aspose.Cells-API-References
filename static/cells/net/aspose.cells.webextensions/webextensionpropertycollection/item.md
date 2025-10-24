##WebExtensionPropertyCollection.Item
WebExtensionPropertyCollection property. Gets the property of web extension by the index
## WebExtensionPropertyCollection indexer (1 of 2)
Gets the property of web extension by the index.
```csharp
public WebExtensionProperty this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The property of web extension.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a web extension property collection
WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
// Add some properties
int index1 = properties.Add("Property1", "Value1");
int index2 = properties.Add("Property2", "Value2");
// Access properties using Item indexer
Console.WriteLine("Property at index 0: Name={0}, Value={1}",
properties[index1].Name, properties[index1].Value);
Console.WriteLine("Property at index 1: Name={0}, Value={1}",
properties[index2].Name, properties[index2].Value);
// Modify property values through the collection
properties[index1].Value = "UpdatedValue1";
properties[index2].Value = "UpdatedValue2";
// Demonstrate the changes
Console.WriteLine("\nAfter modification:");
Console.WriteLine("Property at index 0: Name={0}, Value={1}",
properties[index1].Name, properties[index1].Value);
Console.WriteLine("Property at index 1: Name={0}, Value={1}",
properties[index2].Name, properties[index2].Value);
// Save the workbook (though web extension properties won't be visible in the saved file without proper setup)
workbook.Save("WebExtensionPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
## WebExtensionPropertyCollection indexer (2 of 2)
Gets the property of web extension.
```csharp
public WebExtensionProperty this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of property. |
### Return Value
The property of web extension.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a web extension property collection
WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
// Add properties to the collection
properties.Add("Property1", "Value1");
properties.Add("Property2", "Value2");
// Access properties using the Item indexer
WebExtensionProperty property1 = properties["Property1"];
Console.WriteLine("Property1 value: " + property1.Value);
WebExtensionProperty property2 = properties["Property2"];
Console.WriteLine("Property2 value: " + property2.Value);
// Modify property values (note: Item is read-only, so we need to use Add/Remove)
properties.RemoveAt("Property1");
properties.Add("Property1", "NewValue1");
// Show updated value
property1 = properties["Property1"];
Console.WriteLine("Updated Property1 value: " + property1.Value);
// Save the workbook
workbook.Save("WebExtensionPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
