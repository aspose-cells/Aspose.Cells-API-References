##Cell.GetHtmlString
Cell method. Gets the html string which contains data and some formats in this cell
## Cell.GetHtmlString method
Gets the html string which contains data and some formats in this cell.
```csharp
public string GetHtmlString(bool html5)
```
| Parameter | Type | Description |
| --- | --- | --- |
| html5 | Boolean | Indicates whether the value is compatible for html5 |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetHtmlStringWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample cell value with formatting
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
Style style = cell.GetStyle();
style.Font.Name = "Calibri";
style.Font.Size = 11;
style.Font.Color = System.Drawing.Color.Red;
cell.SetStyle(style);
// Demonstrate GetHtmlString with boolean parameter
string htmlWithoutDiv = cell.GetHtmlString(false);
string htmlWithDiv = cell.GetHtmlString(true);
Console.WriteLine("HTML without div wrapper:");
Console.WriteLine(htmlWithoutDiv);
Console.WriteLine("\nHTML with div wrapper:");
Console.WriteLine(htmlWithDiv);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
