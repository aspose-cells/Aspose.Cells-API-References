##BuiltInDocumentPropertyCollection.Subject
BuiltInDocumentPropertyCollection property. Gets or sets the subject of the document
## BuiltInDocumentPropertyCollection.Subject property
Gets or sets the subject of the document.
```csharp
public string Subject { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties
workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
workbook.BuiltInDocumentProperties.Title = "LiteraTest";
// Save the workbook
string outputPath = "output.xlsx";
workbook.Save(outputPath, SaveFormat.Xlsx);
// Load the saved workbook to verify properties
using (Workbook loadedWorkbook = new Workbook(outputPath))
{
string subject = loadedWorkbook.BuiltInDocumentProperties.Subject;
string title = loadedWorkbook.BuiltInDocumentProperties.Title;
Console.WriteLine("Subject: " + subject);
Console.WriteLine("Title: " + title);
}
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
