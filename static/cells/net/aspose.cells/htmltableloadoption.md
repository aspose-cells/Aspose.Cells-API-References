##Class HtmlTableLoadOption
Aspose.Cells.HtmlTableLoadOption class. Represents the option when import table from html
## HtmlTableLoadOption class
Represents the option when import table from html.
```csharp
public class HtmlTableLoadOption
```
## Constructors
| Name | Description |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Get or set the id of table to import from html |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) Get or set the name of table to import from html |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Get or set the original index of worksheet in the html. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Get or set the index of table to import from html. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Indicates whether generate list objects from imported table. The default value is false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Get or set the target index of worksheet where the table is to be located. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlTableLoadOptionDemo
{
public static void HtmlTableLoadOptionExample()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Create an instance of HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Create an instance of HtmlTableLoadOption
HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
{
TableIndex = 0,
Id = "table1",
Name = "SampleTable",
OriginalSheetIndex = 0,
TargetSheetIndex = 0,
TableToListObject = true
};
// Add the HtmlTableLoadOption to the HtmlLoadOptions
loadOptions.TableLoadOptions.Add(tableLoadOption);
// Load the HTML file into the workbook with the specified load options
workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);
// Save the workbook to an Excel file
workbook.Save("HtmlTableLoadOptionExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
