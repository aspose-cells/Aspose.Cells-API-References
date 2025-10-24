##Class WebExtensionProperty
Aspose.Cells.WebExtensions.WebExtensionProperty class. Represents an Office Addin custom property
## WebExtensionProperty class
Represents an Office Add-in custom property.
```csharp
public class WebExtensionProperty
```
## Properties
| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Gets and set a custom property name. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Gets and sets a custom property value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionsClassWebExtensionPropertyDemo
{
public static void Run()
{
try
{
// Create a new instance of WebExtensionProperty
WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
// Set property values
property.Name = "SampleProperty";
property.Value = "SampleValue";
// Display the property values
Console.WriteLine($"Property Name: {property.Name}");
Console.WriteLine($"Property Value: {property.Value}");
Console.WriteLine("WebExtensionProperty demo completed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
