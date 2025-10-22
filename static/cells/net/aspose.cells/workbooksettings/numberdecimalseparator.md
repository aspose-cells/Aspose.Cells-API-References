##WorkbookSettings.NumberDecimalSeparator
WorkbookSettings property. Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region
## WorkbookSettings.NumberDecimalSeparator property
Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.
```csharp
public char NumberDecimalSeparator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyNumberDecimalSeparatorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
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
