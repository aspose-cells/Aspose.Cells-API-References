##Class PowerQueryFormulaCollection
Aspose.Cells.QueryTables.PowerQueryFormulaCollection class. Represents all power query formulas in the mashup data
## PowerQueryFormulaCollection class
Represents all power query formulas in the mashup data.
```csharp
public class PowerQueryFormulaCollection : CollectionBase<PowerQueryFormula>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulacollection/item/) { get; } | Gets [`PowerQueryFormula`](../powerqueryformula/) by the index in the list. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormula) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormula[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveBy](../../aspose.cells.querytables/powerqueryformulacollection/removeby/)(string) | Remove power query formula by name. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");
// Create a DataMashup object
DataMashup dataMashup = workbook.DataMashup;
// Access PowerQueryFormulas collection
PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;
// Display the count of Power Query formulas
Console.WriteLine($"Number of Power Query Formulas: {powerQueryFormulas.Count}");
// Example of accessing a specific Power Query formula (if any exist)
if (powerQueryFormulas.Count > 0)
{
PowerQueryFormula firstFormula = powerQueryFormulas[0];
Console.WriteLine($"First Power Query Formula: {firstFormula}");
}
// Save the workbook
workbook.Save("PowerQueryFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)
