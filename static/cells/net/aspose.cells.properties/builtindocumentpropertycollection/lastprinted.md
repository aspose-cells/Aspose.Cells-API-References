##BuiltInDocumentPropertyCollection.LastPrinted
BuiltInDocumentPropertyCollection property. Gets or sets the date when the document was last printed in local timezone
## BuiltInDocumentPropertyCollection.LastPrinted property
Gets or sets the date when the document was last printed in local timezone.
```csharp
public DateTime LastPrinted { get; set; }
```
### Remarks
If the document was never printed, this property will return DateTime.MinValue.
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties
workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;
// Display the LastPrinted property
Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
