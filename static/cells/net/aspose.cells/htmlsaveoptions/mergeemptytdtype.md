##HtmlSaveOptions.MergeEmptyTdType
HtmlSaveOptions property. The option to merge contiguous empty cellsempty td elements The default value is MergeEmptyTdType.Default
## HtmlSaveOptions.MergeEmptyTdType property
The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.
```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyMergeEmptyTdTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue(""); // Empty cell
// Configure HTML save options with MergeEmptyTdType
HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
{
MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
};
// Save to HTML
string outputPath = "output.html";
workbook.Save(outputPath, htmlOptions);
Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
}
}
}
```
### See Also
* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
