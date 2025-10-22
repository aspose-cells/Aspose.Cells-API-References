##HtmlTableLoadOption.Id
HtmlTableLoadOption property. Get or set the id of table to import from html
## HtmlTableLoadOption.Id property
Get or set the id of table to import from html
```csharp
public string Id { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionPropertyIdDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Configure table load options
HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
tableLoadOption1.Id = "table1"; // Setting Id property
tableLoadOption1.TargetSheetIndex = 0;
HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
tableLoadOption2.Id = "table2"; // Setting Id property
tableLoadOption2.TargetSheetIndex = 0;
// Add table load options
loadOptions.TableLoadOptions.Add(tableLoadOption1);
loadOptions.TableLoadOptions.Add(tableLoadOption2);
// Load HTML file with specified options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
