##BuiltInDocumentPropertyCollection.LastSavedBy
BuiltInDocumentPropertyCollection property. Gets or sets the name of the last author
## BuiltInDocumentPropertyCollection.LastSavedBy property
Gets or sets the name of the last author.
```csharp
public string LastSavedBy { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties including LastSavedBy
workbook.BuiltInDocumentProperties.Author = "John Doe";
workbook.BuiltInDocumentProperties.Title = "Sample Document";
workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify properties
Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
// Output the LastSavedBy property
Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
