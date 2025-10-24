##ScenarioInputCell.Value
ScenarioInputCell property. Gets and sets value of the input cell
## ScenarioInputCell.Value property
Gets and sets value of the input cell.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scenario
int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
// Add input cells with values
scenario.InputCells.Add(0, 0, "100"); // Cell A1
scenario.InputCells.Add(1, 1, "200"); // Cell B2
// Access and modify values
ScenarioInputCell cell1 = scenario.InputCells[0];
Console.WriteLine($"Original value: {cell1.Value}");
cell1.Value = "150"; // Modify the value
Console.WriteLine($"Modified value: {cell1.Value}");
// Save the workbook
workbook.Save("ScenarioValueDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
