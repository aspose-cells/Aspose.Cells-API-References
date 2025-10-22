##FontSettingCollection.HtmlString
FontSettingCollection property. Gets and sets the html string which contains data and some formats in this shape
## FontSettingCollection.HtmlString property
Gets and sets the html string which contains data and some formats in this shape.
```csharp
public string HtmlString { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionPropertyHtmlStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
var fontSettingCollection = textBox.TextBody;
// Set initial text with HTML formatting
string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
fontSettingCollection.HtmlString = initialHtml;
// Display the current HTML string
Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);
// Modify the HTML string to add more formatting
string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
fontSettingCollection.HtmlString = modifiedHtml;
// Display the modified values
Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);
// Add a cell with HTML formatted text
var cell = worksheet.Cells["A1"];
cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";
// Save the workbook to show both text box and cell HTML formatting
workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
}
}
}
```
### See Also
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
