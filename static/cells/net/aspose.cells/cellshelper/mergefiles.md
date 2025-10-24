##CellsHelper.MergeFiles
CellsHelper method. Merges some large xls files to a xls file
## CellsHelper.MergeFiles method
Merges some large xls files to a xls file.
```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| files | String[] | The files. |
| cachedFile | String | The cached file. |
| destFile | String | The dest file. |
### Remarks
This method only supports merging data, style and formulas to the new file. The cached file is used to store some temporary data.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class CellsHelperMethodMergeFilesWithStringStringDemo
{
public static void Run()
{
// Create temporary Excel files to merge
string[] filesToMerge = new string[2];
filesToMerge[0] = "File1.xlsx";
filesToMerge[1] = "File2.xlsx";
// Create sample workbooks
Workbook workbook1 = new Workbook();
workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
workbook1.Save(filesToMerge[0]);
Workbook workbook2 = new Workbook();
workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
workbook2.Save(filesToMerge[1]);
string cachedFile = "CacheFile.tmp";
string outputFile = "MergedOutput.xlsx";
try
{
// Call MergeFiles with String[], String, String parameters
CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);
Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);
// Verify the merged file
Workbook mergedWorkbook = new Workbook(outputFile);
Console.WriteLine("Merged content:");
Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error merging files: {ex.Message}");
}
finally
{
// Clean up temporary files
if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
if (File.Exists(cachedFile)) File.Delete(cachedFile);
}
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
