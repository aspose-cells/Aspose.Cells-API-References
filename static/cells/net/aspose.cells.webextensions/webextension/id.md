##WebExtension.Id
WebExtension property. Gets and sets the uniquely identifies the Office Addin instance in the current document
## WebExtension.Id property
Gets and sets the uniquely identifies the Office Add-in instance in the current document.
```csharp
public string Id { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Get web extensions collection from workbook
var webExtensions = workbook.Worksheets.WebExtensions;
// Add a new web extension (this will create it with required parameters)
int index = webExtensions.Add();
WebExtension webExtension = webExtensions[index];
// Set the Id property (since it's read-write)
webExtension.Id = "SampleAddin123";
// Display the current value of the Id property
Console.WriteLine($"WebExtension Id: {webExtension.Id}");
// Modify the Id property to demonstrate it's writable
webExtension.Id = "UpdatedAddin456";
Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
// Save the workbook
workbook.Save("WebExtensionIdDemo.xlsx");
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
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
