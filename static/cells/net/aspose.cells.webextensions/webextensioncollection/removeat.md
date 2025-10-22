##WebExtensionCollection.RemoveAt
WebExtensionCollection method. Remove web extension by the index
## WebExtensionCollection.RemoveAt method
Remove web extension by the index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create web extensions collection
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
// Add some web extensions to the collection
int index1 = webExtensions.Add();
int index2 = webExtensions.Add();
int index3 = webExtensions.Add();
Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");
try
{
// Call the RemoveAt method with Int32 parameter
webExtensions.RemoveAt(index2);
Console.WriteLine("Method executed successfully with parameter (Int32)");
Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
// Save the result
workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
