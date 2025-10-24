##BuiltInDocumentPropertyCollection.LinksUpToDate
BuiltInDocumentPropertyCollection property. Indicates whether hyperlinks in a document are uptodate
## BuiltInDocumentPropertyCollection.LinksUpToDate property
Indicates whether hyperlinks in a document are up-to-date.
```csharp
public bool LinksUpToDate { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties collection
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the LinksUpToDate property to indicate if hyperlinks are current
builtInProperties.LinksUpToDate = true;
// Add a simple hyperlink to demonstrate the property
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Save the workbook
workbook.Save("LinksUpToDateDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
