##BuiltInDocumentPropertyCollection.LastPrintedUniversalTime
BuiltInDocumentPropertyCollection property. Gets or sets the Universal time when the document was last printed
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property
Gets or sets the Universal time when the document was last printed.
```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the LastPrintedUniversalTime property
DateTime currentUtcTime = DateTime.UtcNow;
builtInProperties.LastPrintedUniversalTime = currentUtcTime;
// Display the set value
Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);
// Save the workbook
workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
