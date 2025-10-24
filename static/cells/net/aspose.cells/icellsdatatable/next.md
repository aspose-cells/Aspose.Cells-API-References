##ICellsDataTable.Next
ICellsDataTable method. Moves the cursor down one row from its current position
## ICellsDataTable.Next method
Moves the cursor down one row from its current position.
```csharp
public bool Next()
```
### Return Value
if the new current row is valid; false if there are no more rows
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ICellsDataTableMethodNextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
object[][] data = new object[][]
{
new object[] { "Name", "Age", "City" },
new object[] { "John", 25, "New York" },
new object[] { "Anna", 30, "London" },
new object[] { "Peter", 35, "Paris" }
};
try
{
ImportTableOptions importOptions = new ImportTableOptions();
importOptions.IsFieldNameShown = true;
// Create an ICellsDataTable from the data array
ICellsDataTable sourceDataTable = new CellsArrayDataTable(data, importOptions.IsFieldNameShown);
// Import the ICellsDataTable into the worksheet
worksheet.Cells.ImportData(sourceDataTable, 0, 0, importOptions);
ICellsDataTable dataTable = sourceDataTable;
Console.WriteLine("Columns: " + string.Join(", ", dataTable.Columns));
Console.WriteLine("Total Data Rows: " + (dataTable.Count == -1 ? "Unknown" : dataTable.Count.ToString()));
dataTable.BeforeFirst();
Console.WriteLine("\nData Table Contents:");
while (dataTable.Next())
{
Console.WriteLine($"{dataTable[0]}, {dataTable[1]}, {dataTable[2]}");
}
Console.WriteLine("Method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Next method: {ex.Message}");
}
workbook.Save("MethodNextDemo.xlsx");
}
}
// Custom ICellsDataTable implementation for array data
internal class CellsArrayDataTable : ICellsDataTable
{
private readonly object[][] _data;
private readonly bool _hasHeaders;
private int _currentRow = -1;
public CellsArrayDataTable(object[][] data, bool hasHeaders)
{
_data = data;
_hasHeaders = hasHeaders;
}
public string[] Columns
{
get
{
if (_hasHeaders && _data.Length > 0)
{
var headers = new string[_data[0].Length];
for (int i = 0; i < headers.Length; i++)
headers[i] = _data[0][i]?.ToString() ?? "";
return headers;
}
return new string[_data.Length > 0 ? _data[0].Length : 0];
}
}
public int Count => _hasHeaders ? _data.Length - 1 : _data.Length;
public object this[int column] => _data[_currentRow + (_hasHeaders ? 1 : 0)][column];
public object this[string columnName]
{
get
{
int columnIndex = Array.IndexOf(Columns, columnName);
if (columnIndex == -1)
throw new ArgumentException($"Column '{columnName}' not found.");
return this[columnIndex];
}
}
public void BeforeFirst()
{
_currentRow = -1;
}
public bool Next()
{
_currentRow++;
return _currentRow < (_hasHeaders ? _data.Length - 1 : _data.Length);
}
}
}
```
### See Also
* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
