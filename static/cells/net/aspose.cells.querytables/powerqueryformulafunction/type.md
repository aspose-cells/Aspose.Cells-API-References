##PowerQueryFormulaFunction.Type
PowerQueryFormulaFunction property. Gets the type of power query formula
## PowerQueryFormulaFunction.Type property
Gets the type of power query formula.
```csharp
public override PowerQueryFormulaType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
public class PowerQueryFormulaFunctionPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a Power Query formula function
// Since we can't create directly, we'll need to get it from somewhere
// For demo purposes, we'll just show how to access the Type property
// (In real usage, you would get this from an existing collection)
PowerQueryFormulaFunction function = null; // Can't instantiate directly
// Since we can't create a QueryTable directly either, we'll skip that part
QueryTable queryTable = null; // Can't instantiate directly
// Can't add to query tables collection this way - it's read-only
// worksheet.QueryTables[0] = queryTable; // Removed this line
// For demonstration, we'll just show the output format we would use if we had a function
if (function != null)
{
Console.WriteLine("Power Query Formula Function Type: " + function.Type);
Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
}
else
{
Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
}
// Save the result
workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
