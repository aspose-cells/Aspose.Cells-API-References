##Class AutoNumberedBulletValue
Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue class. Represents automatic numbered bullet
## AutoNumberedBulletValue class
Represents automatic numbered bullet.
```csharp
public class AutoNumberedBulletValue : BulletValue
```
## Constructors
| Name | Description |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Represents the scheme of automatic number. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Gets and sets the starting number of the bullet. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Gets the type of the bullet. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextsClassAutoNumberedBulletValueDemo
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
AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
StartAt = 1
};
// Display bullet properties
Console.WriteLine($"Bullet Type: {bullet.Type}");
Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
Console.WriteLine($"Starting Number: {bullet.StartAt}");
// Modify properties
bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
bullet.StartAt = 5;
// Save the workbook
workbook.Save("TextsClassAutoNumberedBulletValueDemo.xlsx");
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
* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
