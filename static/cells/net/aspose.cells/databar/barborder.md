##DataBar.BarBorder
DataBar property. Gets an object that specifies the border of a data bar
## DataBar.BarBorder property
Gets an object that specifies the border of a data bar.
```csharp
public DataBarBorder BarBorder { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyBarBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
sheet.Cells["A4"].PutValue(40);
// Add data bar conditional formatting
int idx = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 3;
area.StartColumn = 0;
area.EndColumn = 0;
fcc.AddArea(area);
// Add data bar condition
int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcc[conditionIdx];
// Set data bar properties
fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
fc.DataBar.Color = Color.Blue;
fc.DataBar.ShowValue = true;
// Set bar border properties
fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
fc.DataBar.BarBorder.Color = Color.Black;
// Save the workbook
workbook.Save("DataBarBorderDemo.xlsx");
}
}
}
```
### See Also
* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
