##WorksheetCollection.BuiltInDocumentProperties
WorksheetCollection property. Returns a DocumentProperty collection that represents all the builtin document properties of the spreadsheet
## WorksheetCollection.BuiltInDocumentProperties property
Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.
```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```
### Remarks
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list:
Title
Subject
Author
Keywords
Comments
Template
Last Author
Revision Number
Application Name
Last Print Date
Creation Date
Last Save Time
Total Editing Time
Number of Pages
Number of Words
Number of Characters
Security
Category
Format
Manager
Company
Number of Bytes
Number of Lines
Number of Paragraphs
Number of Slides
Number of Notes
Number of Hidden Slides
Number of Multimedia Clips
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
authorProperty.Value = "John Smith";
DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
titleProperty.Value = "Sample Document";
Console.WriteLine("Document properties set successfully");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
