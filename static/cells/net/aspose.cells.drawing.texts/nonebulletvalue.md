##Class NoneBulletValue
Aspose.Cells.Drawing.Texts.NoneBulletValue class. Represents no bullet
## NoneBulletValue class
Represents no bullet.
```csharp
public class NoneBulletValue : BulletValue
```
## Constructors
| Name | Description |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Gets the type of the bullet's value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class NoneBulletValueDemo
{
public static void NoneBulletValueExample()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding text to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample text without bullet");
// Create a TextBox to apply bullet settings
Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
textBox.Text = "This is a TextBox without bullet points";
// Create an instance of NoneBulletValue
NoneBulletValue noneBulletValue = new NoneBulletValue();
// Check the type of bullet (should be None)
BulletType bulletType = noneBulletValue.Type;
Console.WriteLine("Bullet Type: " + bulletType); // Output should be None
// Save the workbook to demonstrate the changes
workbook.Save("NoneBulletValueExample.xlsx");
}
}
}
```
### See Also
* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
