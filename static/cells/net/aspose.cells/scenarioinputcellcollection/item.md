##ScenarioInputCellCollection.Item
ScenarioInputCellCollection property. Gets ScenarioInputCell by index in the list
## ScenarioInputCellCollection indexer
Gets [`ScenarioInputCell`](../../scenarioinputcell/) by index in the list.
```csharp
public ScenarioInputCell this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The specific index in the list |
### Return Value
The [`ScenarioInputCell`](../../scenarioinputcell/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioInputCellCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
ScenarioInputCellCollection inputCells = scenario.InputCells;
inputCells.Add(0, 0, "10");
inputCells.Add(1, 1, "20");
// Demonstrate Item property usage
ScenarioInputCell firstCell = inputCells[0];
ScenarioInputCell secondCell = inputCells[1];
Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");
workbook.Save("ScenarioInputCellCollectionExample.xlsx");
}
}
}
```
### See Also
* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
