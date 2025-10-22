##Cell.NumberCategoryType
Cell property. Represents the category type of this cells number formatting
## Cell.NumberCategoryType property
Represents the category type of this cell's number formatting.
```csharp
public NumberCategoryType NumberCategoryType { get; }
```
### Remarks
When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is Number; When cell's value is 0 or not numeric value, the returned type is Text.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyNumberCategoryTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a date value to cell A1
Cell dateCell = worksheet.Cells["A1"];
dateCell.PutValue(DateTime.Now);
// Set date format
Style dateStyle = dateCell.GetStyle();
dateStyle.Custom = "yyyy-mm-dd";
dateCell.SetStyle(dateStyle);
// Add a numeric value to cell A2
Cell numberCell = worksheet.Cells["A2"];
numberCell.PutValue(1234.56);
// Add a text value to cell A3
Cell textCell = worksheet.Cells["A3"];
textCell.PutValue("Sample Text");
// Display NumberCategoryType for each cell
Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
// Change A2 to currency format and check NumberCategoryType
Style currencyStyle = numberCell.GetStyle();
currencyStyle.Custom = "$#,##0.00";
numberCell.SetStyle(currencyStyle);
Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
}
}
}
```
### See Also
* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
