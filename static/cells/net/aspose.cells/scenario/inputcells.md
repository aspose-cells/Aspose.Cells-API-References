##Scenario.InputCells
Scenario property. Gets the input cells of scenario
## Scenario.InputCells property
Gets the input cells of scenario.
```csharp
public ScenarioInputCellCollection InputCells { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyInputCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scenario to the worksheet
int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
// Add input cells to the scenario using InputCells property
ScenarioInputCellCollection inputCells = scenario.InputCells;
inputCells.Add(0, 0, "100"); // Cell A1
inputCells.Add(1, 1, "200"); // Cell B2
// Modify the first input cell's value
inputCells[0].Value = "150";
// Save the workbook
workbook.Save("ScenarioInputCellsDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
