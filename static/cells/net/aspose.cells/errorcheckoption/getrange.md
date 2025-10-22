##ErrorCheckOption.GetRange
ErrorCheckOption method. Gets the influenced range of this setting by given index
## ErrorCheckOption.GetRange method
Gets the influenced range of this setting by given index.
```csharp
public CellArea GetRange(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of range |
### Return Value
return influenced range at given index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ErrorCheckOptionMethodGetRangeWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an ErrorCheckOption using the worksheet's ErrorCheckOptions collection
int errorCheckIndex = worksheet.ErrorCheckOptions.Add();
ErrorCheckOption errorCheckOption = worksheet.ErrorCheckOptions[errorCheckIndex];
CellArea area = new CellArea();
area.StartRow = 1;
area.StartColumn = 1;
area.EndRow = 3;
area.EndColumn = 3;
int addedIndex = errorCheckOption.AddRange(area);
try
{
int rangeCount = errorCheckOption.GetCountOfRange();
if (rangeCount > 0)
{
CellArea retrievedArea = errorCheckOption.GetRange(0);
Console.WriteLine($"Retrieved range: StartRow={retrievedArea.StartRow}, StartColumn={retrievedArea.StartColumn}, " +
$"EndRow={retrievedArea.EndRow}, EndColumn={retrievedArea.EndColumn}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRange method: {ex.Message}");
}
workbook.Save("ErrorCheckOptionMethodGetRangeWithInt32Demo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
