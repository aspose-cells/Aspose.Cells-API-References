##TextOptions.LanguageCode
TextOptions property. Gets and sets the user interface language
## TextOptions.LanguageCode property
Gets and sets the user interface language.
```csharp
public CountryCode LanguageCode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextOptionsPropertyLanguageCodeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set its text
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
shape.Text = "Sample text with language settings";
// Set the language code for the shape's text options
shape.TextOptions.LanguageCode = CountryCode.Japan;
// Verify and output the language code
Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);
// Save the workbook
workbook.Save("TextOptionsLanguageDemo.xlsx");
}
}
}
```
### See Also
* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
