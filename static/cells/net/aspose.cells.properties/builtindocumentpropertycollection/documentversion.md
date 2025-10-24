##BuiltInDocumentPropertyCollection.DocumentVersion
BuiltInDocumentPropertyCollection property. Represents the version of the file
## BuiltInDocumentPropertyCollection.DocumentVersion property
Represents the version of the file.
```csharp
public string DocumentVersion { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set document version property
workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
// Display the document version
Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
// Save the workbook
workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
