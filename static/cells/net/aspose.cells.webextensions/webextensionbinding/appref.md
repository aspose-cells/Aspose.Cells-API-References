##WebExtensionBinding.Appref
WebExtensionBinding property. Gets and sets the binding key used to map the binding entry in this list with the bound data in the document
## WebExtensionBinding.Appref property
Gets and sets the binding key used to map the binding entry in this list with the bound data in the document.
```csharp
public string Appref { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionBindingPropertyApprefDemo
{
public static void Run()
{
try
{
// Create a new WebExtensionBinding instance
WebExtensionBinding binding = new WebExtensionBinding();
// Set properties including Appref
binding.Id = "Binding1";
binding.Type = "text";
binding.Appref = "Sheet1!A1:B2";
// Display the current value of Appref
Console.WriteLine("Appref value: " + binding.Appref);
// Modify the Appref value to demonstrate it's read/write
binding.Appref = "Sheet1!C3:D4";
Console.WriteLine("Updated Appref value: " + binding.Appref);
Console.WriteLine("Appref property has been successfully demonstrated");
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
* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
