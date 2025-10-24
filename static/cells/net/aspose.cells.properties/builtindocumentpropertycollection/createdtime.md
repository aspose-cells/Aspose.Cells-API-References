##BuiltInDocumentPropertyCollection.CreatedTime
BuiltInDocumentPropertyCollection property. Gets or sets date of the document creation in local timezone
## BuiltInDocumentPropertyCollection.CreatedTime property
Gets or sets date of the document creation in local timezone.
```csharp
public DateTime CreatedTime { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyCreatedTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the CreatedTime property to current time
DateTime currentTime = DateTime.Now;
workbook.BuiltInDocumentProperties.CreatedTime = currentTime;
// Save the workbook
string outputPath = "output_CreatedTimeDemo.xlsx";
workbook.Save(outputPath);
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook(outputPath);
DateTime loadedTime = loadedWorkbook.BuiltInDocumentProperties.CreatedTime;
Console.WriteLine("Original CreatedTime: " + currentTime);
Console.WriteLine("Loaded CreatedTime: " + loadedTime);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
