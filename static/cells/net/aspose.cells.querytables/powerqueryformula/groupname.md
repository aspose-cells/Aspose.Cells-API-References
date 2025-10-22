##PowerQueryFormula.GroupName
PowerQueryFormula property. Gets the name of group which contains this power query formula
## PowerQueryFormula.GroupName property
Gets the name of group which contains this power query formula.
```csharp
public string GroupName { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaPropertyGroupNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a Power Query formula (simulated since we can't create actual PowerQueryFormulas directly)
// Normally you would load from an existing file with Power Query formulas
string sourcePath = "example.xlsx";
try
{
workbook = new Workbook(sourcePath);
PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
if (queries.Count > 0)
{
Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
// Demonstrate accessing the GroupName property
string groupName = queries[0].GroupName;
Console.WriteLine($"Group Name: {groupName}");
// Save and reload to demonstrate persistence
string destPath = "output.xlsx";
workbook.Save(destPath);
Workbook workbook2 = new Workbook(destPath);
PowerQueryFormulaCollection queries2 = workbook2.DataMashup.PowerQueryFormulas;
if (queries2.Count > 0)
{
Console.WriteLine("After reload - Group Name: " + queries2[0].GroupName);
}
}
else
{
Console.WriteLine("No Power Query formulas found in the file.");
}
}
catch (Exception ex)
{
Console.WriteLine("Error: " + ex.Message);
Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
}
}
}
}
```
### See Also
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
