##HtmlSaveOptions.MergeEmptyTdForcely
HtmlSaveOptions property. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html please keep the default value
## HtmlSaveOptions.MergeEmptyTdForcely property
Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.
```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
{
public static void Run()
{
// Create a sample workbook with empty cells
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create some empty cells in the worksheet
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
// B2 is intentionally left empty
// Save with MergeEmptyTdForcely enabled
HtmlSaveOptions options = new HtmlSaveOptions();
options.MergeEmptyTdForcely = true;
workbook.Save("output_with_merge.html", options);
// Save without MergeEmptyTdForcely for comparison
options.MergeEmptyTdForcely = false;
workbook.Save("output_without_merge.html", options);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
