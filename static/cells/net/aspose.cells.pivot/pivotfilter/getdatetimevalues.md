##PivotFilter.GetDateTimeValues
PivotFilter method. Gets values of the number filter
## PivotFilter.GetDateTimeValues method
Gets values of the number filter.
```csharp
public DateTime[] GetDateTimeValues()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterMethodGetDateTimeValuesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Date";
cells["B1"].Value = "Sales";
cells["A2"].Value = DateTime.Now;
cells["B2"].Value = 1000;
cells["A3"].Value = DateTime.Now.AddDays(1);
cells["B3"].Value = 2000;
cells["A4"].Value = DateTime.Now.AddDays(2);
cells["B4"].Value = 3000;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field and apply date filter
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.BaseFields[0].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
// Get the filter and demonstrate GetDateTimeValues
PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
DateTime[] dateValues = filter.GetDateTimeValues();
Console.WriteLine("Filter Type: " + filter.FilterType);
Console.WriteLine("First Date Value: " + dateValues[0]);
Console.WriteLine("Second Date Value: " + dateValues[1]);
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
