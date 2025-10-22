##BuiltInDocumentPropertyCollection.RevisionNumber
BuiltInDocumentPropertyCollection property. Gets or sets the document revision number
## BuiltInDocumentPropertyCollection.RevisionNumber property
Gets or sets the document revision number.
```csharp
public string RevisionNumber { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the RevisionNumber property
workbook.BuiltInDocumentProperties.RevisionNumber = "1";
// Display the RevisionNumber
Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
