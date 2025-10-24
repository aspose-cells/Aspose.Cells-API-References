##ScenarioInputCell.Name
ScenarioInputCell property. Gets and sets the input cell address
## ScenarioInputCell.Name property
Gets and sets the input cell address.
```csharp
public string Name { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a scenario
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex = scenarios.Add("TestScenario");
// Get the scenario
Scenario scenario = scenarios[scenarioIndex];
// Add input cells to the scenario
ScenarioInputCellCollection inputCells = scenario.InputCells;
inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)
// Get the input cells
ScenarioInputCell inputCell1 = inputCells[0];
ScenarioInputCell inputCell2 = inputCells[1];
// Demonstrate Name property usage
Console.WriteLine("First input cell name: " + inputCell1.Name);
Console.WriteLine("Second input cell name: " + inputCell2.Name);
// Verify the names match expected values
if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
{
throw new Exception("Input cell names don't match expected values");
}
}
}
}
```
### See Also
* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
