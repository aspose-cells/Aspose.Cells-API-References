##PivotFilter.GetNumberValues
PivotFilter method. Gets values of the number filter
## PivotFilter.GetNumberValues method
Gets values of the number filter.
```csharp
public double[] GetNumberValues()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterMethodGetNumberValuesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 5;
sheet.Cells["B3"].Value = 3;
sheet.Cells["B4"].Value = 2;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.RefreshData();
pivotTable.CalculateData();
// Apply value filter
pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
// Get and display filter values
PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
double[] numberValues = filter.GetNumberValues();
Console.WriteLine("Filter Type: " + filter.FilterType);
Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
