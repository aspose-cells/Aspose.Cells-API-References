##WebExtensionProperty.Value
WebExtensionProperty property. Gets and sets a custom property value
## WebExtensionProperty.Value property
Gets and sets a custom property value.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionPropertyPropertyValueDemo
{
public static void Run()
{
try
{
// Create a WebExtensionProperty instance
WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
// Set and demonstrate Value property
property.Value = "SampleValue123";
Console.WriteLine($"Initial Value: {property.Value}");
// Modify and show updated value
property.Value = "UpdatedValue456";
Console.WriteLine($"Modified Value: {property.Value}");
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
