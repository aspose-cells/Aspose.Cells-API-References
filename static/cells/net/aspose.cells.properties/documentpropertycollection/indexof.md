##DocumentPropertyCollection.IndexOf
DocumentPropertyCollection method. Gets the index of a property by name
## DocumentPropertyCollection.IndexOf method
Gets the index of a property by name.
```csharp
public int IndexOf(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |
### Return Value
The zero based index. Negative value if not found.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the built-in document properties collection
DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
// For built-in properties, we can only set values of existing properties
// To add custom properties, we would need to use CustomDocumentPropertyCollection
// Here we'll just set some existing built-in properties for demonstration
properties["Title"].Value = "Value1";
properties["Subject"].Value = "Value2";
properties["Author"].Value = "Value3";
try
{
// Call the IndexOf method with string parameter
int index = properties.IndexOf("Subject");
// Display the result
Console.WriteLine($"Index of 'Subject': {index}");
// Show the property at found index
if (index >= 0)
{
DocumentProperty property = properties[index];
Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
}
// Save the workbook
workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
}
}
}
```
### See Also
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
