##WebExtensionBinding.Id
WebExtensionBinding property. Gets and sets the binding identifier
## WebExtensionBinding.Id property
Gets and sets the binding identifier.
```csharp
public string Id { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionBindingPropertyIdDemo
{
public static void Run()
{
try
{
// Create a new WebExtensionBinding instance
WebExtensionBinding binding = new WebExtensionBinding();
// Set the Id property
binding.Id = "SampleBindingId";
// Display the current value of Id
Console.WriteLine("Initial Id value: " + binding.Id);
// Modify the Id value to demonstrate it's read/write
binding.Id = "UpdatedBindingId";
Console.WriteLine("Updated Id value: " + binding.Id);
Console.WriteLine("Id property has been successfully demonstrated");
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
