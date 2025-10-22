##LightCellsDataHandler.StartRow
LightCellsDataHandler method. Prepares to process a row
## LightCellsDataHandler.StartRow method
Prepares to process a row.
```csharp
public bool StartRow(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | the index of next row to be processed |
### Return Value
whether this row(properties or cells data) needs to be processed. false to ignore this row and its cells and check the next row.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataHandlerMethodStartRowWithInt32Demo
{
public static void Run()
{
try
{
using (Workbook workbook = new Workbook())
{
Worksheet sheet = workbook.Worksheets[0];
for (int i = 0; i < 5; i++)
{
sheet.Cells[i, 0].Value = $"Row {i + 1}";
}
workbook.Save("input.xlsx");
}
LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
using (Workbook workbook = new Workbook("input.xlsx", loadOptions))
{
workbook.Save("output.xlsx");
}
Console.WriteLine("Method executed successfully. Rows with even indices processed.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing StartRow: {ex.Message}");
}
}
private class CustomLightCellsDataHandler : LightCellsDataHandler
{
public bool StartRow(int rowIndex)
{
return rowIndex % 2 == 0;
}
public bool StartSheet(Worksheet sheet) => true;
public bool ProcessRow(Row row) => true;
public bool StartCell(int columnIndex) => true;
public bool ProcessCell(Cell cell) => true;
}
}
}
```
### See Also
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
