##DocumentPropertyCollection.Contains
DocumentPropertyCollection method. Returns true if a property with the specified name exists in the collection
## DocumentPropertyCollection.Contains method
Returns true if a property with the specified name exists in the collection.
```csharp
public bool Contains(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |
### Return Value
True if the property exists in the collection; false otherwise.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocumentPropertyCollectionMethodContainsWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Check if "RevisionNumber" property exists in built-in document properties
bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
// Add a custom property and check for its existence
workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
}
}
}
```
### See Also
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
