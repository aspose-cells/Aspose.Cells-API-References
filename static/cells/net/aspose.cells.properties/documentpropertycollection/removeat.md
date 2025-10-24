##DocumentPropertyCollection.RemoveAt
DocumentPropertyCollection method. Removes a property at the specified index
## DocumentPropertyCollection.RemoveAt method
Removes a property at the specified index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The zero based index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access custom document properties (instead of built-in)
DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
// Add some custom properties to demonstrate removal
((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");
try
{
// Display properties before removal
Console.WriteLine("Properties before removal:");
foreach (DocumentProperty prop in properties)
{
Console.WriteLine($"{prop.Name}: {prop.Value}");
}
// Call RemoveAt with index 1 (second property)
properties.RemoveAt(1);
// Display properties after removal
Console.WriteLine("\nProperties after removal:");
foreach (DocumentProperty prop in properties)
{
Console.WriteLine($"{prop.Name}: {prop.Value}");
}
Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Error: Index out of range. {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
// Save the workbook
workbook.Save("RemoveAtMethodDemo.xlsx");
}
}
}
```
### See Also
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
