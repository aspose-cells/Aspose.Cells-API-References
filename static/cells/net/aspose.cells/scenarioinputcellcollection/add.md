##ScenarioInputCellCollection.Add
ScenarioInputCellCollection method. Adds an input cell
## ScenarioInputCellCollection.Add method
Adds an input cell.
```csharp
public int Add(int row, int column, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index of input cell. |
| column | Int32 | The column index of input cell. |
| value | String | The value of input cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellCollectionMethodAddWithInt32Int32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
ScenarioInputCellCollection inputCells = scenario.InputCells;
inputCells.Add(0, 0, "10");
inputCells.Add(1, 1, "20");
Console.WriteLine($"Count: {inputCells.Count}");
Console.WriteLine($"Cell 1: Row={inputCells[0].Row}, Column={inputCells[0].Column}, Value={inputCells[0].Value}");
Console.WriteLine($"Cell 2: Row={inputCells[1].Row}, Column={inputCells[1].Column}, Value={inputCells[1].Value}");
workbook.Save("ScenarioInputCellCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
