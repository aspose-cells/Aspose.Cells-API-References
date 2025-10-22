##Class ScenarioInputCellCollection
Aspose.Cells.ScenarioInputCellCollection class. Represents the list of the scenarios input cells
## ScenarioInputCellCollection class
Represents the list of the scenario's input cells.
```csharp
public class ScenarioInputCellCollection : CollectionBase<ScenarioInputCell>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenarioinputcellcollection/item/) { get; } | Gets [`ScenarioInputCell`](../scenarioinputcell/) by index in the list. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/scenarioinputcellcollection/add/)(int, int, string) | Adds an input cell. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ScenarioInputCell) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ScenarioInputCell, IComparer&lt;ScenarioInputCell&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ScenarioInputCell, IComparer&lt;ScenarioInputCell&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ScenarioInputCell) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ScenarioInputCell[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ScenarioInputCell[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ScenarioInputCell[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ScenarioInputCellCollectionDemo
{
public static void ScenarioInputCellCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scenario to the worksheet
int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
Scenario scenario = worksheet.Scenarios[scenarioIndex];
// Access the ScenarioInputCellCollection
ScenarioInputCellCollection inputCells = scenario.InputCells;
// Add input cells to the scenario
inputCells.Add(0, 0, "10"); // Adding cell A1 with value 10
inputCells.Add(1, 1, "20"); // Adding cell B2 with value 20
// Access and print the properties of the ScenarioInputCellCollection
Console.WriteLine("Capacity: " + inputCells.Capacity);
Console.WriteLine("Count: " + inputCells.Count);
// Access individual ScenarioInputCell by index
ScenarioInputCell inputCell1 = inputCells[0];
ScenarioInputCell inputCell2 = inputCells[1];
// Print details of the input cells
Console.WriteLine($"Input Cell 1: Row={inputCell1.Row}, Column={inputCell1.Column}, Value={inputCell1.Value}");
Console.WriteLine($"Input Cell 2: Row={inputCell2.Row}, Column={inputCell2.Column}, Value={inputCell2.Value}");
// Save the workbook
workbook.Save("ScenarioInputCellCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ScenarioInputCell](../scenarioinputcell/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
