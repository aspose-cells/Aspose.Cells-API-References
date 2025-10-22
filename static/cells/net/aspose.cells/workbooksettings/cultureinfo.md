##WorkbookSettings.CultureInfo
WorkbookSettings property. Gets or sets the system culture info
## WorkbookSettings.CultureInfo property
Gets or sets the system culture info.
```csharp
public CultureInfo CultureInfo { get; set; }
```
### Remarks
Returns null if culture info is not set and [`Region`](../region/) is not set.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyCultureInfoDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Set region to France to demonstrate CultureInfo changes
wb.Settings.Region = CountryCode.France;
// Get the group separator from French culture
string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
Console.WriteLine($"French group separator: '{groupSep}'");
// Create a style with custom format and show culture-adjusted format
Style style = wb.CreateStyle();
style.Custom = "#,##0.00_ ;-#,##0.00";
Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
// Demonstrate number formatting with French culture
Worksheet sheet = wb.Worksheets[0];
Cell cell = sheet.Cells["A1"];
cell.PutValue(123456.78);
cell.SetStyle(style);
style.Custom = "# ###,00 €";
Console.WriteLine($"Formatted value: {cell.StringValue}");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
