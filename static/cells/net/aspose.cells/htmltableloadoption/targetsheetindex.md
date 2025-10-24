##HtmlTableLoadOption.TargetSheetIndex
HtmlTableLoadOption property. Get or set the target index of worksheet where the table is to be located
## HtmlTableLoadOption.TargetSheetIndex property
Get or set the target index of worksheet where the table is to be located.
```csharp
public int TargetSheetIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Configure table load options with TargetSheetIndex
HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
tableLoadOption1.Id = "table1";
tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
tableLoadOption2.Id = "table2";
tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
// Add table load options
loadOptions.TableLoadOptions.Add(tableLoadOption1);
loadOptions.TableLoadOptions.Add(tableLoadOption2);
// Load HTML file with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the tables were loaded to correct sheets
Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
