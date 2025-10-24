##SpreadsheetSplitter.Process
SpreadsheetSplitter method. Splits given template file into multiple parts
## Process(string, string) {#process_1}
Splits given template file into multiple parts.
```csharp
public static void Process(string templateFile, string resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be split |
| resultFile | String | The resultant file(name pattern) |
### Remarks
The output files will be build from the specified resultant file by appending sequence number of the sheet and split part. For example, if the specified output file is Split.xlsx, then the generated files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class SpreadsheetSplitterMethodProcessWithStringStringDemo
{
public static void Run()
{
// Create a new workbook with multiple worksheets
Workbook templateWorkbook = new Workbook();
Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
sheet1.Cells["A1"].PutValue("Product");
Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
sheet2.Cells["A1"].PutValue("test data");
// Save as template file
string templatePath = "SplitterTemplate.xlsx";
templateWorkbook.Save(templatePath, SaveFormat.Xlsx);
// Define result output pattern
string resultPattern = "SplitResult_";
try
{
// Process template directly using the static method
SpreadsheetSplitter.Process(templatePath, resultPattern);
Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
Console.WriteLine("Check output directory for split files");
}
catch (Exception ex)
{
Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
}
}
}
}
```
### See Also
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeSplitOptions) {#process}
Splits spreadsheet file into multiple parts.
```csharp
public static void Process(LowCodeSplitOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | LowCodeSplitOptions | Options for splitting spreadsheet |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
{
public static void Run()
{
// Initialize split options
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
{
LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
};
try
{
// Execute spreadsheet splitting using static method
SpreadsheetSplitter.Process(splitOptions);
Console.WriteLine($"Spreadsheet split successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Split operation failed: {ex.Message}");
}
}
}
// Concrete implementation of AbstractLowCodeSaveOptionsProvider
public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override void Finish(LowCodeSaveOptions part)
{
base.Finish(part);
}
// Implement the required abstract method
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
{
if (partInfo == null)
{
throw new ArgumentNullException(nameof(partInfo));
}
LowCodeSaveOptions result = new LowCodeSaveOptions();
result.SaveFormat = SaveFormat.Xlsx;
result.OutputFile = partInfo.SheetName + "_split.xlsx";
Console.WriteLine(result.OutputFile);
return result;
}
}
}
```
### See Also
* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
