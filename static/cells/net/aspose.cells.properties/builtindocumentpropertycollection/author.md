##BuiltInDocumentPropertyCollection.Author
BuiltInDocumentPropertyCollection property. Gets or sets the name of the documents author
## BuiltInDocumentPropertyCollection.Author property
Gets or sets the name of the document's author.
```csharp
public string Author { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the author property
string authorName = "John Doe";
workbook.BuiltInDocumentProperties.Author = authorName;
// Display the author property
Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);
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
