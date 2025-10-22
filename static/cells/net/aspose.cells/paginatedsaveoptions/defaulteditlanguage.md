##PaginatedSaveOptions.DefaultEditLanguage
PaginatedSaveOptions property. Gets or sets default edit language
## PaginatedSaveOptions.DefaultEditLanguage property
Gets or sets default edit language.
```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```
### Remarks
It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some CJK text to demonstrate the DefaultEditLanguage property
worksheet.Cells["A1"].PutValue("日本語のテキスト");
worksheet.Cells["A2"].PutValue("中文文本");
worksheet.Cells["A3"].PutValue("한글 텍스트");
// Create PDF save options and set CJK as default edit language
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
// Save the workbook with the specified options
workbook.Save("output.pdf", pdfSaveOptions);
Console.WriteLine("Workbook saved with CJK as default edit language.");
}
}
}
```
### See Also
* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
