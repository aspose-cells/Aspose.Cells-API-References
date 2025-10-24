##PaginatedSaveOptions.CheckFontCompatibility
PaginatedSaveOptions property. Indicates whether to check font compatibility for every character in text
## PaginatedSaveOptions.CheckFontCompatibility property
Indicates whether to check font compatibility for every character in text.
```csharp
public bool CheckFontCompatibility { get; set; }
```
### Remarks
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Font Compatibility Test");
// Create paginated save options
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Demonstrate CheckFontCompatibility property
saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
// Set other required properties
saveOptions.DefaultFont = "Arial";
saveOptions.CheckWorkbookDefaultFont = true;
// Save the document with the specified options
workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
Console.WriteLine("Document saved with CheckFontCompatibility = false");
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
