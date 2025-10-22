##BuiltInDocumentPropertyCollection.Item
BuiltInDocumentPropertyCollection property. Returns a DocumentProperty object by the name of the property
## BuiltInDocumentPropertyCollection indexer
Returns a [`DocumentProperty`](../../documentproperty/) object by the name of the property.
```csharp
public override DocumentProperty this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The case-insensitive name of the property to retrieve. |
### Remarks
The string names of the properties correspond to the names of the typed properties available from [`BuiltInDocumentPropertyCollection`](../).
If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [`DocumentProperty`](../../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).
If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set a built-in document property using the proper method
workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
// Access and print the property value
Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook and verify the property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
