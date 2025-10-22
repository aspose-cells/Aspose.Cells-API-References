##ExportTableOptions.PreprocessExportedValue
ExportTableOptions method. Preprocess the value of current cell to be exported
## ExportTableOptions.PreprocessExportedValue method
Preprocess the value of current cell to be exported.
```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellRow | Int32 | the row index of current cell |
| cellColumn | Int32 | the column index of cell |
| value | CellValue | value and type of current cell |
### Return Value
Whether current cell has been replaced with different type and/or value.
### Remarks
The row and column index is cell's absolute index in the worksheet, not index in the exported table. User may check the value of current cell in the override implementation of this method, if current cell needs to be replaced with other type and value, here the implementation should set the expected type and value to the CellValue object and return true. By default this method does nothing and returns false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in the worksheet
worksheet.Cells["A1"].PutValue("Test Value");
worksheet.Cells["A2"].PutValue(123.45);
worksheet.Cells["A3"].PutValue(DateTime.Now);
// Create an instance of ExportTableOptions
ExportTableOptions exportOptions = new ExportTableOptions();
// Create a CellValue object for demonstration
CellValue cellValue = new CellValue();
cellValue.Type = CellValueType.IsString;
cellValue.Value = "Processed Value";
try
{
// Call PreprocessExportedValue with specific parameters (row 0, column 0, CellValue)
bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);
// Display the result of the method call
Console.WriteLine($"PreprocessExportedValue returned: {result}");
// Modify the cell with the processed value if needed
if (result)
{
worksheet.Cells[0, 0].PutValue(cellValue.Value);
}
// Save the workbook
workbook.Save("PreprocessExportedValueDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
