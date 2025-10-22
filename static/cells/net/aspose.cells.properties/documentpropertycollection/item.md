##DocumentPropertyCollection.Item
DocumentPropertyCollection property. Returns a DocumentProperty object by the name of the property
## DocumentPropertyCollection indexer (1 of 2)
Returns a [`DocumentProperty`](../../documentproperty/) object by the name of the property.
```csharp
public virtual DocumentProperty this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The case-insensitive name of the property to retrieve. |
### Remarks
Returns null if a property with the specified name is not found.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocumentPropertyCollectionPropertyItemDemo
{
public static void Run()
{
Workbook wb = new Workbook();
string key = "TemplateGUID";
object value = "TestValue123";
if (wb.Worksheets.CustomDocumentProperties.Contains(key))
{
wb.Worksheets.CustomDocumentProperties[key].Value = value;
}
else
{
wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
}
// Verify the value was set using Item property
Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## DocumentPropertyCollection indexer (2 of 2)
Returns a [`DocumentProperty`](../../documentproperty/) object by index.
```csharp
public DocumentProperty this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | Zero-based index of the [`DocumentProperty`](../../documentproperty/) to retrieve. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Set built-in properties (not Add)
properties.Author = "John Doe";
properties.Company = "Aspose";
properties["Version"].Value = "1.0";
// Access properties using Item indexer
Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);
// Access property by name
DocumentProperty authorProp = properties["Author"];
Console.WriteLine("Author property: " + authorProp.Value);
// Modify a property
properties["Version"].Value = "2.0";
Console.WriteLine("Updated Version: " + properties["Version"].Value);
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
