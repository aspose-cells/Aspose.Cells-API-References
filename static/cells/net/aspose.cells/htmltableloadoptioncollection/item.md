##HtmlTableLoadOptionCollection.Item
HtmlTableLoadOptionCollection property. Gets the HtmlTableLoadOption element at the specified index
## HtmlTableLoadOptionCollection indexer
Gets the [`HtmlTableLoadOption`](../../htmltableloadoption/) element at the specified index.
```csharp
public HtmlTableLoadOption this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionPropertyItemDemo
{
public static void Run()
{
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a new HtmlTableLoadOption by table index
int index1 = tableLoadOptions.Add(0);
// Access the HtmlTableLoadOption using Item property
HtmlTableLoadOption option = tableLoadOptions[index1];
// Configure the table load option
option.TableToListObject = true;
option.TargetSheetIndex = 1;
// Load HTML file with the configured options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
