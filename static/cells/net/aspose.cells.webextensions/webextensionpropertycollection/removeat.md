##WebExtensionPropertyCollection.RemoveAt
WebExtensionPropertyCollection method. Remove the property by the name
## WebExtensionPropertyCollection.RemoveAt method
Remove the property by the name.
```csharp
public void RemoveAt(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a web extension property collection
WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
// Add some properties to the collection
properties.Add("Property1", "Value1");
properties.Add("Property2", "Value2");
properties.Add("Property3", "Value3");
try
{
// Call the RemoveAt method with string parameter
properties.RemoveAt("Property2");
Console.WriteLine("Property with name 'Property2' removed successfully.");
// Display remaining properties
Console.WriteLine("Remaining properties:");
for (int i = 0; i < properties.Count; i++)
{
Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
// Save the workbook
workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
