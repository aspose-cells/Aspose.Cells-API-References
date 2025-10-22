##HtmlTableLoadOption.OriginalSheetIndex
HtmlTableLoadOption property. Get or set the original index of worksheet in the html
## HtmlTableLoadOption.OriginalSheetIndex property
Get or set the original index of worksheet in the html.
```csharp
public int OriginalSheetIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionPropertyOriginalSheetIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
{
TableIndex = 0,
OriginalSheetIndex = 1,
TargetSheetIndex = 0
};
loadOptions.TableLoadOptions.Add(tableLoadOption);
workbook = new Workbook("input.html", loadOptions);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
