##PictureBulletValue.Type
PictureBulletValue property. Gets the type of the bullets value
## PictureBulletValue.Type property
Gets the type of the bullet's value.
```csharp
public override BulletType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class PictureBulletValuePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create an instance of PictureBulletValue
PictureBulletValue bulletValue = new PictureBulletValue();
// Display the Type property value (read-only operation)
Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
// Demonstrate that the Type is correctly set to Picture for this class
if (bulletValue.Type == BulletType.Picture)
{
Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
}
// Save the workbook
workbook.Save("PictureBulletValueTypeDemo.xlsx");
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
* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
