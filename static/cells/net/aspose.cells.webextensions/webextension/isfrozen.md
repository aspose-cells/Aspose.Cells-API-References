##WebExtension.IsFrozen
WebExtension property. Indicates whether the user can interact with the Office Addin or not
## WebExtension.IsFrozen property
Indicates whether the user can interact with the Office Add-in or not.
```csharp
public bool IsFrozen { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyIsFrozenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// This line will fail because WebExtension requires constructor parameters
// WebExtension webExtension = new WebExtension();
// Instead, we'll get a web extension from the workbook if possible
// or demonstrate with a different approach
Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
// For demonstration purposes, we'll show how the property would work if you had a valid instance
// In a real scenario, you would get the WebExtension instance from the workbook or another source
WebExtension webExtension = GetWebExtensionInstance(workbook);
if (webExtension != null)
{
// Set initial properties
webExtension.Id = "MyAddin123";
// Display initial IsFrozen value
Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
// Change the IsFrozen property (since it's read-write)
webExtension.IsFrozen = true;
Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
// Demonstrate effect by checking if user can interact
Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
// Save the workbook (though web extension might not be persisted without additional steps)
workbook.Save("WebExtensionIsFrozenDemo.xlsx");
}
else
{
Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
private static WebExtension GetWebExtensionInstance(Workbook workbook)
{
// In a real implementation, this would get an existing WebExtension from the workbook
// or create one properly with required constructor parameters
// This is just a placeholder for demonstration
return null;
}
}
}
```
### See Also
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
