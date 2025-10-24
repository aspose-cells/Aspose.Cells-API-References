##SpreadsheetMerger.Process
SpreadsheetMerger method. Merge given template files
## Process(string[], string) {#process_1}
Merge given template files.
```csharp
public static void Process(string[] templateFiles, string resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFiles | String[] | The template files to be merged |
| resultFile | String | The resultant file |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
{
public static void Run()
{
// Create sample template files
CreateTemplateFile("template1.xlsx", "Data from Template 1");
CreateTemplateFile("template2.xlsx", "Data from Template 2");
string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
string resultFile = "merged_output.xlsx";
try
{
SpreadsheetMerger.Process(templateFiles, resultFile);
Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Process method: {ex.Message}");
}
}
private static void CreateTemplateFile(string fileName, string cellValue)
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
workbook.Save(fileName);
}
}
}
```
### See Also
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeMergeOptions) {#process}
Merges multiple template files into one.
```csharp
public static void Process(LowCodeMergeOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | LowCodeMergeOptions | Options for merging files |
### See Also
* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
