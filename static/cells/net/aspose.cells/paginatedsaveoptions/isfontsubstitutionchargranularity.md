##PaginatedSaveOptions.IsFontSubstitutionCharGranularity
PaginatedSaveOptions property. Indicates whether to only substitute the font of character when the cell font is not compatibility for it
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```
### Remarks
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyIsFontSubstitutionCharGranularityDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Sample Text with Font Substitution");
XpsSaveOptions saveOptions = new XpsSaveOptions
{
IsFontSubstitutionCharGranularity = true,
DefaultFont = "Arial"
};
workbook.Save("FontSubstitutionDemo.xps", saveOptions);
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
