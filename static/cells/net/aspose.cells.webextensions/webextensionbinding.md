##Class WebExtensionBinding
Aspose.Cells.WebExtensions.WebExtensionBinding class. Represents a binding relationship between an Office Addin and the data in the document
## WebExtensionBinding class
Represents a binding relationship between an Office Add-in and the data in the document.
```csharp
public class WebExtensionBinding
```
## Constructors
| Name | Description |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Gets and sets the binding identifier. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Gets and sets the binding type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionsClassWebExtensionBindingDemo
{
public static void Run()
{
try
{
// Create a new WebExtensionBinding instance
WebExtensionBinding binding = new WebExtensionBinding();
// Set properties
binding.Id = "DemoBinding";
binding.Type = "range";
binding.Appref = "Sheet1!A1";
// Display property values
Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");
// Modify properties
binding.Appref = "Sheet1!B2";
Console.WriteLine($"Updated Appref: {binding.Appref}");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
