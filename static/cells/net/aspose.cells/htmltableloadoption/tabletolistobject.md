##HtmlTableLoadOption.TableToListObject
HtmlTableLoadOption property. Indicates whether generate list objects from imported table. The default value is false
## HtmlTableLoadOption.TableToListObject property
Indicates whether generate list objects from imported table. The default value is false.
```csharp
public bool TableToListObject { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionPropertyTableToListObjectDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Create HTML load options with TableToListObject enabled
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
{
TableIndex = 0,
TableToListObject = true
};
loadOptions.TableLoadOptions.Add(tableLoadOption);
// Load HTML with the specified options
workbook = new Workbook("input.html", loadOptions);
// Save as Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
