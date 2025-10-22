##BuiltInDocumentPropertyCollection.Language
BuiltInDocumentPropertyCollection property. Gets or sets the documents language
## BuiltInDocumentPropertyCollection.Language property
Gets or sets the document's language.
```csharp
public string Language { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties collection
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the language property
builtInProperties.Language = "en-US";
// Set other basic properties for demonstration
builtInProperties.Author = "John Doe";
builtInProperties.Title = "Language Property Demo";
// Save the workbook
workbook.Save("LanguagePropertyDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
