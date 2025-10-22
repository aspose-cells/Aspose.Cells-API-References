##PowerQueryFormula.PowerQueryFormulaItems
PowerQueryFormula property. Gets all items of power query formula
## PowerQueryFormula.PowerQueryFormulaItems property
Gets all items of power query formula.
```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
{
public static void Run()
{
// Load the source workbook
Workbook workbook = new Workbook("example.xlsx");
// Access the first Power Query formula and its first item
PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
// Modify the item value (replace drive letter)
string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
item.Value = modifiedValue;
// Save the workbook
workbook.Save("modified_example.xlsx");
// Verify the change
Console.WriteLine("Original value modified to: " + modifiedValue);
}
}
}
```
### See Also
* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
