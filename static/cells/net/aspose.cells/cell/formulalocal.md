##Cell.FormulaLocal
Cell property. Get the locale formatted formula of the cell
## Cell.FormulaLocal property
Get the locale formatted formula of the cell.
```csharp
public string FormulaLocal { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyFormulaLocalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set default locale to German for demonstration
workbook.Settings.Region = CountryCode.Germany;
// Access cell A1
Cell cell = worksheet.Cells["A1"];
// Set formula in standard format (English)
cell.Formula = "=SUM(B1:C1)";
// Display formulas in both standard and local formats
Console.WriteLine("Standard Formula: " + cell.Formula);
Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
// Set formula in local format (German)
cell.FormulaLocal = "=SUMME(B1:C1)";
// Display formulas again to show the difference
Console.WriteLine("\nAfter setting FormulaLocal:");
Console.WriteLine("Standard Formula: " + cell.Formula);
Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
// Demonstrate GetFormula with localization
Console.WriteLine("\nUsing GetFormula:");
Console.WriteLine("English formula: " + cell.GetFormula(false, false));
Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
