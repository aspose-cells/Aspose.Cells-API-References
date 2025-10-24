##HtmlTableLoadOption.Name
HtmlTableLoadOption property. Get or set the name of table to import from html
## HtmlTableLoadOption.Name property
Get or set the name of table to import from html
```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionPropertyNameDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a new HtmlTableLoadOption by table index
int index = tableLoadOptions.Add(0);
// Access the HtmlTableLoadOption
HtmlTableLoadOption option = tableLoadOptions[index];
// Set the Name property
option.Name = "CustomerDataTable";
// Load an HTML file (replace with actual file path)
workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
