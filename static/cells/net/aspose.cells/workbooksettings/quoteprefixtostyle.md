##WorkbookSettings.QuotePrefixToStyle
WorkbookSettings property. Indicates whether setting QuotePrefix property when entering the string valuewhich starts with single quote mark  to the cell
## WorkbookSettings.QuotePrefixToStyle property
Indicates whether setting [`QuotePrefix`](../../style/quoteprefix/) property when entering the string value(which starts with single quote mark ) to the cell
```csharp
public bool QuotePrefixToStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyQuotePrefixToStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Enable QuotePrefixToStyle - strings starting with ' will have QuotePrefix style applied
workbook.Settings.QuotePrefixToStyle = true;
Cell cell1 = workbook.Worksheets[0].Cells["A1"];
cell1.PutValue("'abc");
Console.WriteLine("Cell A1 - QuotePrefix: " + cell1.GetStyle().QuotePrefix);
Console.WriteLine("Cell A1 - Value: " + cell1.StringValue);
// Disable QuotePrefixToStyle - strings keep their literal value
workbook.Settings.QuotePrefixToStyle = false;
Cell cell2 = workbook.Worksheets[0].Cells["A2"];
cell2.PutValue("'abc");
Console.WriteLine("Cell A2 - QuotePrefix: " + cell2.GetStyle().QuotePrefix);
Console.WriteLine("Cell A2 - Value: " + cell2.StringValue);
workbook.Save("QuotePrefixToStyleDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
