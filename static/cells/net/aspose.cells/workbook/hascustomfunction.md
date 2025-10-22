##Workbook.HasCustomFunction
Workbook property. Detects whether there is custom function used in this workbook such as in cells formula in defined names
## Workbook.HasCustomFunction property
Detects whether there is custom function used in this workbook, such as in cell's formula, in defined names...
```csharp
public bool HasCustomFunction { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyHasCustomFunctionDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add a standard formula to a name
NameCollection names = wb.Worksheets.Names;
int index = names.Add("StandardName");
names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");
// Add a custom function to a name
index = names.Add("CustomName");
names[index].RefersTo = "=MYFUNC()";
Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");
// Test with cell formulas
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Standard function in cell
cells["A1"].Formula = "=SUM(B1:B2)";
Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");
// Custom function in cell
cells["A2"].Formula = "=MYFUNC(B1)";
Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");
// Reference to name with custom function
cells["A3"].Formula = "=CustomName";
Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");
// Combined custom functions
cells["A4"].Formula = "=MYFUNC(CustomName)";
Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
