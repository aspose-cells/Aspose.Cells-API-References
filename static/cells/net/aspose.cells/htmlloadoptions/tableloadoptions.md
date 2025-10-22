##HtmlLoadOptions.TableLoadOptions
HtmlLoadOptions property. Get the HtmlTableLoadOptionCollection instance
## HtmlLoadOptions.TableLoadOptions property
Get the HtmlTableLoadOptionCollection instance
```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
loadOptions.SupportDivTag = true;
// Add table load options by index
loadOptions.TableLoadOptions.Add(1);
loadOptions.TableLoadOptions.Add(2);
// Add table load options by ID
HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
tableLoadOption.Id = "table1";
loadOptions.TableLoadOptions.Add(tableLoadOption);
tableLoadOption = new HtmlTableLoadOption();
tableLoadOption.Id = "table2";
loadOptions.TableLoadOptions.Add(tableLoadOption);
// Load HTML file with the options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the output
workbook.Save("output.xlsx");
// Clear and add new table load options
loadOptions.TableLoadOptions.Clear();
// Add table load options with sheet index mapping
loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
// Add table load options with ID and sheet mapping
tableLoadOption = new HtmlTableLoadOption();
tableLoadOption.Id = "mainTable";
tableLoadOption.TargetSheetIndex = 1;
loadOptions.TableLoadOptions.Add(tableLoadOption);
// Load and save again with new options
workbook = new Workbook("input.html", loadOptions);
workbook.Save("output_mapped.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
