##BuiltInDocumentPropertyCollection.NameOfApplication
BuiltInDocumentPropertyCollection property. Gets or sets the name of the application
## BuiltInDocumentPropertyCollection.NameOfApplication property
Gets or sets the name of the application.
```csharp
public string NameOfApplication { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the NameOfApplication property
workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
// Display the NameOfApplication property
Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
// Save the workbook
workbook.Save("output.ods");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
