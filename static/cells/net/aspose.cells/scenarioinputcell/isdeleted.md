##ScenarioInputCell.IsDeleted
ScenarioInputCell property. Indicates whether input cell is deleted
## ScenarioInputCell.IsDeleted property
Indicates whether input cell is deleted.
```csharp
public bool IsDeleted { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellPropertyIsDeletedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scenario
int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
// Add input cells
ScenarioInputCellCollection inputCells = scenario.InputCells;
inputCells.Add(0, 0, "100");
inputCells.Add(1, 1, "200");
// Access and display input cells
ScenarioInputCell cell1 = inputCells[0];
Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");
// Delete the first input cell
cell1.IsDeleted = true;
Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");
// Save the workbook
workbook.Save("ScenarioWithDeletedCell.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
