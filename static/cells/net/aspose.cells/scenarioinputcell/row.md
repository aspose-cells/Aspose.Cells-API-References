##ScenarioInputCell.Row
ScenarioInputCell property. Gets and sets the row index of the input cell
## ScenarioInputCell.Row property
Gets and sets the row index of the input cell.
```csharp
public int Row { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scenario to the worksheet
int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
// Add input cells to the scenario
scenario.InputCells.Add(0, 0, "10"); // Cell A1
scenario.InputCells.Add(1, 1, "20"); // Cell B2
// Access and demonstrate Row property
ScenarioInputCell cell1 = scenario.InputCells[0];
Console.WriteLine($"First input cell is at row: {cell1.Row}");
// Add a new cell at row 2 instead of trying to modify the existing one
worksheet.Cells[2, 0].Value = "30"; // Cell A3
scenario.InputCells.Add(2, 0, "30");
Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");
// Save the workbook
workbook.Save("ScenarioInputCellRowDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
