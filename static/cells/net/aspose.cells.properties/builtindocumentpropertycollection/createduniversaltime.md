##BuiltInDocumentPropertyCollection.CreatedUniversalTime
BuiltInDocumentPropertyCollection property. Gets or sets the Universal time of the document creation
## BuiltInDocumentPropertyCollection.CreatedUniversalTime property
Gets or sets the Universal time of the document creation.
```csharp
public DateTime CreatedUniversalTime { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyCreatedUniversalTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the CreatedUniversalTime property
DateTime creationTime = new DateTime(2023, 5, 15, 15, 30, 0, DateTimeKind.Utc);
workbook.BuiltInDocumentProperties.CreatedUniversalTime = creationTime;
// Display the CreatedUniversalTime property
Console.WriteLine("Document created (UTC): " +
workbook.BuiltInDocumentProperties.CreatedUniversalTime.ToString());
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
