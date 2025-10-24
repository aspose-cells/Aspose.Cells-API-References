##ScenarioCollection.Item
ScenarioCollection property. Gets the Scenario object by the index
## ScenarioCollection indexer
Gets the [`Scenario`](../../scenario/) object by the index.
```csharp
public Scenario this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The specific index in the list. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
scenario.InputCells.Add(0, 0, "100");
scenario.InputCells.Add(1, 1, "200");
// Demonstrate Item property usage
ScenarioInputCell firstCell = scenario.InputCells[0];
Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
workbook.Save("ScenarioCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
