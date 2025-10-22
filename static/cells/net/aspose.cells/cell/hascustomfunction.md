##Cell.HasCustomFunction
Cell property. Checks whether there is custom functionunsupported function in this cells formula
## Cell.HasCustomFunction property
Checks whether there is custom function(unsupported function) in this cell's formula.
```csharp
public bool HasCustomFunction { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyHasCustomFunctionDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Add a custom function name
NameCollection nc = wb.Worksheets.Names;
nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
// Access first worksheet
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Test with built-in function
Cell cell1 = cells[0, 0];
cell1.Formula = "=SUM(A1:B1)";
Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
// Test with custom function
Cell cell2 = cells[1, 0];
cell2.Formula = "=MYTESTFUNC()";
Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
// Test with named range containing custom function
Cell cell3 = cells[2, 0];
cell3.Formula = "=MyCustomFunc";
Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
// Test with nested custom function
Cell cell4 = cells[3, 0];
cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
