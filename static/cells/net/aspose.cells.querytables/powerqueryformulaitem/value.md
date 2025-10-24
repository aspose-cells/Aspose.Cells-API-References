##PowerQueryFormulaItem.Value
PowerQueryFormulaItem property. Gets the value of the item
## PowerQueryFormulaItem.Value property
Gets the value of the item.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaItemPropertyValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook("source.xlsx");
foreach (PowerQueryFormula formula in workbook.DataMashup.PowerQueryFormulas)
{
foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
{
if (item.Name == "Source")
{
item.Value = item.Value.Replace("Parameter1", "\"TESTING\"");
}
}
}
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
