##NoneBulletValue.Type
NoneBulletValue property. Gets the type of the bullets value
## NoneBulletValue.Type property
Gets the type of the bullet's value.
```csharp
public override BulletType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class NoneBulletValuePropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
NoneBulletValue noneBulletValue = new NoneBulletValue();
BulletType bulletType = noneBulletValue.Type;
Console.WriteLine("Bullet Type: " + bulletType); // Output: None
workbook.Save("NoneBulletValueExample.xlsx");
}
}
}
```
### See Also
* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
