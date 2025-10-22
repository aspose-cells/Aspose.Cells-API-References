##PowerQueryFormulaCollection.RemoveBy
PowerQueryFormulaCollection method. Remove power query formula by name
## PowerQueryFormulaCollection.RemoveBy method
Remove power query formula by name.
```csharp
public void RemoveBy(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of power query formula. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the PowerQueryFormulaCollection (assuming it exists in the workbook)
PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
// Add a sample formula to be removed (this would normally come from existing data)
string formulaName = "SampleFormula";
// Call RemoveBy with the formula name
powerQueryFormulas.RemoveBy(formulaName);
Console.WriteLine($"Formula '{formulaName}' removed successfully");
// Save the workbook
workbook.Save("RemoveByWithStringDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
}
}
}
}
```
### See Also
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
