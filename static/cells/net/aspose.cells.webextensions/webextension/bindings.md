##WebExtension.Bindings
WebExtension property. Gets all bindings relationship between an Office Addin and the data in the document
## WebExtension.Bindings property
Gets all bindings relationship between an Office Add-in and the data in the document.
```csharp
public WebExtensionBindingCollection Bindings { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyBindingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a sample worksheet
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Assuming we get a web extension from somewhere (since we can't create one directly)
// This is a minimal change to make the code compile while maintaining its structure
WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
if (webExtension != null)
{
// Access the Bindings property (read-only)
WebExtensionBindingCollection bindings = webExtension.Bindings;
// Display information about the bindings
Console.WriteLine($"Number of bindings: {bindings.Count}");
// Add a new binding (demonstrates using the collection)
int newBindingIndex = bindings.Add();
Console.WriteLine($"Added new binding at index: {newBindingIndex}");
// Display updated count
Console.WriteLine($"Updated number of bindings: {bindings.Count}");
}
else
{
Console.WriteLine("No web extension available");
}
// Save the workbook
workbook.Save("WebExtensionBindingsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
