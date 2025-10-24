##WebExtensionReferenceCollection.Item
WebExtensionReferenceCollection property. Gets web extension by the specific index
## WebExtensionReferenceCollection indexer
Gets web extension by the specific index.
```csharp
public WebExtensionReference this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The web extension
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionReferenceCollectionPropertyItemDemo
{
public static void Run()
{
try
{
// Create a new WebExtensionReferenceCollection
WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
// Add a new web extension reference
int index = references.Add();
// Access the Item property (read-only) to get the reference at specified index
WebExtensionReference reference = references[index];
// Display information about the retrieved reference
Console.WriteLine($"Retrieved web extension reference at index: {index}");
Console.WriteLine($"Reference type: {reference.GetType().Name}");
// Note: The Item property is read-only, so we only demonstrate getting its value
}
catch (Exception ex)
{
Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
}
}
}
}
```
### See Also
* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
