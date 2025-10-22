##AutoNumberedBulletValue.AutonumberScheme
AutoNumberedBulletValue property. Represents the scheme of automatic number
## AutoNumberedBulletValue.AutonumberScheme property
Represents the scheme of automatic number.
```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
{
public static void Run()
{
try
{
// Create a new AutoNumberedBulletValue instance
AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();
// Display initial AutonumberScheme value
Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");
// Set a new AutonumberScheme value
bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");
// Create a workbook to demonstrate the bullet in context
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape with text that will use the bullet style
TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
shape.TextBody.Text = "Sample text with bullet formatting";
// Note: Actual application of bullet style to text would require additional API calls
// not shown in the reflection. We'll just save the workbook as demonstration.
workbook.Save("AutonumberSchemeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
