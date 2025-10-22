##Cell.HtmlString
Cell property. Gets and sets the html string which contains data and some formats in this cell
## Cell.HtmlString property
Gets and sets the html string which contains data and some formats in this cell.
```csharp
public string HtmlString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyHtmlStringDemo
{
public static void Run()
{
// Create a workbook instance
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cells collection
Cells cells = worksheet.Cells;
// Set HTML string with formatting to cell A1
cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
// Save the workbook
workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
