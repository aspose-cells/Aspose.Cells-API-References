##WebExtension.AlterReferences
WebExtension property. Gets a list of alter references
## WebExtension.AlterReferences property
Gets a list of alter references.
```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyAlterReferencesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Get web extensions collection from workbook
var webExtensions = workbook.Worksheets.WebExtensions;
// Add a new web extension
int index = webExtensions.Add();
WebExtension webExtension = webExtensions[index];
// Access the AlterReferences property (read-only)
WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
// Display information about the alter references
Console.WriteLine($"Number of alter references: {alterReferences.Count}");
// Add a new alter reference (demonstrates using the collection)
int newRefIndex = alterReferences.Add();
Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
// Display updated count
Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
// Save the workbook
workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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
* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
