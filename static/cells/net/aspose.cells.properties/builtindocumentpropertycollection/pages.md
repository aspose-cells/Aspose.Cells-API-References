##BuiltInDocumentPropertyCollection.Pages
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of pages in the document
## BuiltInDocumentPropertyCollection.Pages property
Represents an estimate of the number of pages in the document.
```csharp
public int Pages { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the Pages property
builtInProperties.Pages = 10;
// Add a worksheet and some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Page Count Demonstration");
worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");
// Save the workbook
workbook.Save("DocumentPagesDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
