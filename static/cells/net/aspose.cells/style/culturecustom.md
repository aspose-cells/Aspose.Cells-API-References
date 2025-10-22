##Style.CultureCustom
Style property. Gets and sets the culturedependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
## Style.CultureCustom property
Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.
```csharp
public string CultureCustom { get; set; }
```
### Remarks
For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyCultureCustomDemo
{
public static void Run()
{
// Create a workbook and set Hungarian culture
Workbook wb = new Workbook();
wb.Settings.CultureInfo = new CultureInfo("hu-HU");
// Get the first cell and its style
Cell cell = wb.Worksheets[0].Cells[0, 0];
Style style = cell.GetStyle();
// Set custom format and demonstrate CultureCustom conversion
string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
style.Custom = customFormat;
Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
style.CultureCustom = cultureCustomFormat;
Console.WriteLine("Custom from CultureCustom: " + style.Custom);
// Apply the style and demonstrate culture-aware formatting
cell.SetStyle(style);
cell.PutValue(47512); // January 29, 2030
Console.WriteLine("Formatted value: " + cell.StringValue);
// Demonstrate formula with culture formatting
cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
wb.CalculateFormula();
Console.WriteLine("Calculated value: " + cell.StringValue);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
