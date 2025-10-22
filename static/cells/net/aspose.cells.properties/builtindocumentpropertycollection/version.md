##BuiltInDocumentPropertyCollection.Version
BuiltInDocumentPropertyCollection property. Represents the version number of the application that created the document
## BuiltInDocumentPropertyCollection.Version property
Represents the version number of the application that created the document.
```csharp
public string Version { get; set; }
```
### Remarks
It's format is "00.0000",for example : 12.0000
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set some document properties
workbook.BuiltInDocumentProperties.Author = "Test Author";
workbook.BuiltInDocumentProperties.Title = "Test Document";
// Access and display the Version property
string version = workbook.BuiltInDocumentProperties.Version;
Console.WriteLine("Document Version: " + version);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
