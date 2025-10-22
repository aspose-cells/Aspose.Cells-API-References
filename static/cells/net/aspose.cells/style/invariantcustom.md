##Style.InvariantCustom
Style property. Gets the cultureindependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
## Style.InvariantCustom property
Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.
```csharp
public string InvariantCustom { get; }
```
### Remarks
For builtin number formats, the returned pattern content is still culture-dependent, such as, for some locales it returns "m/d/y" and for some other locales it returns "d/m/y". The difference from [`CultureCustom`](../culturecustom/) is(that is also what culture-independent means): the format specifiers and separators are kept as standard, such as '/' will always be used as datetime separator and "y" will always be used as the "year" part no matter what other special character is used for the specific locale.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyInvariantCustomDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.Germany;
Cell cell = wb.Worksheets[0].Cells[0, 0];
Style style = cell.GetStyle();
// Set date format and value
style.Number = 14; // Date format
style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
cell.PutValue(new DateTime(2019, 10, 12));
cell.SetStyle(style);
// Output results
Console.WriteLine("Formatted value: " + cell.StringValue);
Console.WriteLine("CultureCustom: " + style.CultureCustom);
Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
