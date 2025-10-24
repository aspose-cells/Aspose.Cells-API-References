##ISmartMarkerCallBack.Process
ISmartMarkerCallBack method. Callback for processing a smart marker
## ISmartMarkerCallBack.Process method
Callback for processing a smart marker.
```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The sheet index. |
| rowIndex | Int32 | The row index. |
| colIndex | Int32 | The column index. |
| tableName | String | The table name of smartmarker. |
| columnName | String | The table name of smartmarker. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo : ISmartMarkerCallBack
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo callback =
new ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo();
try
{
// Call Process method with sample parameters
callback.Process(0, 5, 3, "Products", "ProductName");
Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
// Set a value to show the effect
worksheet.Cells[5, 3].PutValue("ProcessedValue");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Process method: {ex.Message}");
}
workbook.Save("ISmartMarkerCallBackProcessDemo.xlsx");
}
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
{
// Implementation of the Process method
Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
}
}
}
```
### See Also
* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
