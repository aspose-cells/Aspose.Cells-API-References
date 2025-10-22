##PowerQueryFormulaItemCollection.Item
PowerQueryFormulaItemCollection property. Gets PowerQueryFormulaItem by the index in the list
## PowerQueryFormulaItemCollection indexer (1 of 2)
Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the index in the list.
```csharp
public PowerQueryFormulaItem this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaItemCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook with a template that contains Power Query
Workbook workbook = new Workbook();
// Get the first Power Query formula (assuming one exists)
var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
// Modify the formula items using Item property
var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
if (formulaItems.Count > 0)
{
formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
// Verify the change
Console.WriteLine(formulaItems[0].Value);
}
// Save the workbook
workbook.Save("PowerQueryExample.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
## PowerQueryFormulaItemCollection indexer (2 of 2)
Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the name of the item.
```csharp
public PowerQueryFormulaItem this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the item. |
### See Also
* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
