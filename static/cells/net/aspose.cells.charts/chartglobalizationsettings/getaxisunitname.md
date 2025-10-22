##ChartGlobalizationSettings.GetAxisUnitName
ChartGlobalizationSettings method. Gets the Name of Axis Unit
## ChartGlobalizationSettings.GetAxisUnitName method
Gets the Name of Axis Unit.
```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Create globalization settings and get axis unit name
ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);
// Output results
Console.WriteLine("Thousands unit name: " + thousandsUnit);
Console.WriteLine("Millions unit name: " + millionsUnit);
// Save workbook
workbook.Save("AxisUnitNameDemo.xlsx");
}
}
}
```
### See Also
* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
