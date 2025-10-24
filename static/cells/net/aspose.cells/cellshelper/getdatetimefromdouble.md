##CellsHelper.GetDateTimeFromDouble
CellsHelper method. Convert the double value to the date time value
## CellsHelper.GetDateTimeFromDouble method
Convert the double value to the date time value.
```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Double | The double value. |
| date1904 | Boolean | Date 1904 system. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Double, Boolean)
double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
bool date1904 = false; // Using 1900 date system
try
{
// Call the GetDateTimeFromDouble method with the specific parameter types
DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
// Display the result
Console.WriteLine($"Converted DateTime: {result}");
// Write the result to a cell
worksheet.Cells["A1"].PutValue("Original Double Value:");
worksheet.Cells["B1"].PutValue(doubleValue);
worksheet.Cells["A2"].PutValue("Converted DateTime:");
worksheet.Cells["B2"].PutValue(result.ToString());
Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
