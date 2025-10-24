##Cell.GetFormatConditions
Cell method. Gets format conditions which applies to this cell
## Cell.GetFormatConditions method
Gets format conditions which applies to this cell.
```csharp
public FormatConditionCollection[] GetFormatConditions()
```
### Return Value
Returns [`FormatConditionCollection`](../../formatconditioncollection/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetFormatConditionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get cells collection
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
cells["A3"].PutValue(30);
// Add format condition to cell A1
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
fcc.AddArea(area);
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
// Get format conditions for cell A1
FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
// Output the number of format conditions
Console.WriteLine("Number of format conditions: " + conditions.Length);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
