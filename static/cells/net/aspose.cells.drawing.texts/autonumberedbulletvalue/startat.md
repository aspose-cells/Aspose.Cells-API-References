##AutoNumberedBulletValue.StartAt
AutoNumberedBulletValue property. Gets and sets the starting number of the bullet
## AutoNumberedBulletValue.StartAt property
Gets and sets the starting number of the bullet.
```csharp
public int StartAt { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class AutoNumberedBulletValuePropertyStartAtDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an AutoNumberedBulletValue instance
AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
{
AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
StartAt = 3 // Setting the StartAt property
};
// Display the current StartAt value
Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");
// Modify the StartAt value
bullet.StartAt = 5;
Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");
// Create a shape to demonstrate the bullet in context
var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
shape.TextBody.Text = "1. First Item\n2. Second Item";
// Apply the bullet style (note: actual application method not shown in reflection)
// For demonstration, we'll just save the workbook
workbook.Save("StartAtPropertyDemo.xlsx");
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
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
