##LowCodeSaveOptionsProviderOfAssembling.PathTail
LowCodeSaveOptionsProviderOfAssembling property. Tailing partafter sequence numbers of file path. It should include extension of file name
## LowCodeSaveOptionsProviderOfAssembling.PathTail property
Tailing part(after sequence numbers) of file path. It should include extension of file name.
```csharp
public string PathTail { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
{
public static void Run()
{
// Create workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 25; i++)
{
worksheet.Cells[i, 0].Value = $"Record {i + 1}";
}
// Initialize save options provider
var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "SalesReports/Q3",
PathTail = ".xlsx",
UseSheetName = true,
SaveOptionsTemplate = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Xlsx
}
};
Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");
// First save with default extension
workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);
// Modify path tail for CSV output
optionsProvider.PathTail = "_split.csv";
optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");
// Second save with new extension
workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);
Console.WriteLine("Check output directories for generated file formats");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
