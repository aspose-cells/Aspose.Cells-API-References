##BuiltInDocumentPropertyCollection.LastSavedTime
BuiltInDocumentPropertyCollection property. Gets or sets the time of the last save in local timezone
## BuiltInDocumentPropertyCollection.LastSavedTime property
Gets or sets the time of the last save in local timezone.
```csharp
public DateTime LastSavedTime { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties
workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;
// Display the LastSavedTime property
Console.WriteLine("Last Saved Time: " +
workbook.BuiltInDocumentProperties.LastSavedTime);
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
