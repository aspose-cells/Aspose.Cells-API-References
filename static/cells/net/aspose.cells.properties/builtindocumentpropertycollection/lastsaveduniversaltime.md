##BuiltInDocumentPropertyCollection.LastSavedUniversalTime
BuiltInDocumentPropertyCollection property. Gets or sets the universal time of the last save
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property
Gets or sets the universal time of the last save.
```csharp
public DateTime LastSavedUniversalTime { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the LastSavedUniversalTime property
DateTime utcNow = DateTime.UtcNow;
builtInProperties.LastSavedUniversalTime = utcNow;
// Display the set value
Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);
// Save the workbook
workbook.Save("LastSavedUniversalTimeDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
