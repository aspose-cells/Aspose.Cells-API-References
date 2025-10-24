##WebExtensionProperty.Name
WebExtensionProperty property. Gets and set a custom property name
## WebExtensionProperty.Name property
Gets and set a custom property name.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyPropertyNameDemo
{
public static void Run()
{
try
{
// Create a WebExtensionProperty instance
WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
// Set and demonstrate Name property
property.Name = "SampleName";
Console.WriteLine($"Initial Name: {property.Name}");
// Modify and display updated name
property.Name = "UpdatedName";
Console.WriteLine($"Modified Name: {property.Name}");
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
* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
