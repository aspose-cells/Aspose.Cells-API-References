##WebExtensionBindingCollection.Item
WebExtensionBindingCollection property. Gets web extension binding relationship by the specific index
## WebExtensionBindingCollection indexer
Gets web extension binding relationship by the specific index.
```csharp
public WebExtensionBinding this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The web extension binding relationship
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using System;
public class WebExtensionBindingCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a web extension binding collection
WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();
// Add a new binding to the collection
int index = bindingCollection.Add();
// Access the binding using the Item property (read-only)
WebExtensionBinding binding = bindingCollection[index];
// Set properties on the binding
binding.Id = "binding1";
binding.Type = "Text";
binding.Appref = "Sheet1!A1";
// Display the binding details
Console.WriteLine("Binding ID: " + binding.Id);
Console.WriteLine("Binding Type: " + binding.Type);
Console.WriteLine("Binding AppRef: " + binding.Appref);
// Modify the binding through the collection
bindingCollection[index].Id = "modifiedBinding";
Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);
// Save the workbook
workbook.Save("WebExtensionBindingDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
