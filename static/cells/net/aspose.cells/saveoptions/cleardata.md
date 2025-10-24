##SaveOptions.ClearData
SaveOptions property. Make the workbook empty after saving the file
## SaveOptions.ClearData property
Make the workbook empty after saving the file.
```csharp
public bool ClearData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyClearDataDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add test data
worksheet.Cells["A1"].PutValue("Tabelle1");
worksheet.Cells["B3"].PutValue(3);
// Configure save options with ClearData = false
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.ClearData = false;
saveOptions.Separator = ',';
// Save the workbook
string outputPath = "output_with_cleardata_false.csv";
workbook.Save(outputPath, saveOptions);
// Reload to verify data was preserved
Workbook loadedWorkbook = new Workbook(outputPath);
Cells cells = loadedWorkbook.Worksheets[0].Cells;
Console.WriteLine("A1 value: " + cells["A1"].StringValue);
Console.WriteLine("B3 value: " + cells["B3"].IntValue);
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
