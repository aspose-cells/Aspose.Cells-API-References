##WebExtensionBinding.Type
WebExtensionBinding property. Gets and sets the binding type
## WebExtensionBinding.Type property
Gets and sets the binding type.
```csharp
public string Type { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionBindingPropertyTypeDemo
{
public static void Run()
{
try
{
// Create a new WebExtensionBinding instance
WebExtensionBinding binding = new WebExtensionBinding();
// Set the Type property
binding.Type = "text";
// Display the current value of Type
Console.WriteLine("Initial Type value: " + binding.Type);
// Modify the Type value to demonstrate it's read/write
binding.Type = "range";
Console.WriteLine("Updated Type value: " + binding.Type);
Console.WriteLine("Type property has been successfully demonstrated");
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
