##WorkbookSettings.NumberGroupSeparator
WorkbookSettings property. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region
## WorkbookSettings.NumberGroupSeparator property
Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.
```csharp
public char NumberGroupSeparator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyNumberGroupSeparatorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.USA;
wb.Settings.NumberDecimalSeparator = ',';
wb.Settings.NumberGroupSeparator = '.';
Style style = wb.CreateStyle();
style.Custom = "#,##0.00";
Cell cell = wb.Worksheets[0].Cells[0, 0];
cell.PutValue(12345.6798);
cell.SetStyle(style);
Console.WriteLine("Formatted value: " + cell.StringValue);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
