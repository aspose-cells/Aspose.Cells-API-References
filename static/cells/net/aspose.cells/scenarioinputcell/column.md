##ScenarioInputCell.Column
ScenarioInputCell property. Gets and sets the column index of the input cell
## ScenarioInputCell.Column property
Gets and sets the column index of the input cell.
```csharp
public int Column { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellPropertyColumnDemo
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
// Access and demonstrate Column property
ScenarioInputCell cell1 = scenario.InputCells[0];
Console.WriteLine($"First input cell is at column: {cell1.Column}");
// Since Column is read-only, we need to remove and re-add to change column
string value = cell1.Value;
scenario.InputCells.RemoveAt(0);
scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value
// Verify the change
cell1 = scenario.InputCells[0];
Console.WriteLine($"Modified first input cell column to: {cell1.Column}");
// Save the workbook
workbook.Save("ScenarioInputCellColumnDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
