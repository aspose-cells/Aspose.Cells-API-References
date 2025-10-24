##BuiltInDocumentPropertyCollection.TotalEditingTime
BuiltInDocumentPropertyCollection property. Gets or sets the total editing time in minutes
## BuiltInDocumentPropertyCollection.TotalEditingTime property
Gets or sets the total editing time in minutes.
```csharp
public double TotalEditingTime { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the total editing time in minutes
builtInProperties.TotalEditingTime = 90.5;
// Display the set editing time
Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");
// Save the workbook
workbook.Save("TotalEditingTimeDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
