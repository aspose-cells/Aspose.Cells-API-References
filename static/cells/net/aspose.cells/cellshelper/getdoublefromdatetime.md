##CellsHelper.GetDoubleFromDateTime
CellsHelper method. Convert the date time to double value
## CellsHelper.GetDoubleFromDateTime method
Convert the date time to double value.
```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | The date time. |
| date1904 | Boolean | Date 1904 system. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
{
public static void Run()
{
// Create a workbook instance
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get current date and time
DateTime now = DateTime.Now;
// Convert DateTime to double using CellsHelper
double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
// Set the value in cell A1
worksheet.Cells["A1"].PutValue(dateDouble);
// Format the cell to display as date
Style style = worksheet.Cells["A1"].GetStyle();
style.Number = 14; // Date format
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("DateTimeConversionDemo.xlsx");
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
