##Worksheet.SparklineGroups
Worksheet property. Gets the sparkline groups in the worksheet
## Worksheet.SparklineGroups property
Gets the sparkline groups in the worksheet.
```csharp
public SparklineGroupCollection SparklineGroups { get; }
```
### Examples
```csharp
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertySparklineGroupsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Populate test data
Cells cells = sheet.Cells;
for (int i = 0; i < 4; i++)
{
for (int j = 0; j < 4; j++)
{
cells[i, j].Value = (i + 1) * (j + 1);
}
}
// Add sparkline group
int groupIndex = sheet.SparklineGroups.Add(
0, // Line sparkline type code
"A1:D4",
false,
CellArea.CreateCellArea("F1", "F4")
);
workbook.Save("output_sparklines.xlsx");
}
}
}
```
### See Also
* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
