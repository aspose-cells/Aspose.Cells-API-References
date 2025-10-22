##CharacterBulletValue.Type
CharacterBulletValue property. Gets the type of the bullet
## CharacterBulletValue.Type property
Gets the type of the bullet.
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
public class CharacterBulletValuePropertyTypeDemo
{
public static void Run()
{
try
{
// Create a new CharacterBulletValue instance
CharacterBulletValue bulletValue = new CharacterBulletValue();
// Demonstrate the Type property (read-only)
Console.WriteLine("Bullet Type: " + bulletValue.Type);
// Show that the Type is Character for CharacterBulletValue
Console.WriteLine("Is Character bullet type: " +
(bulletValue.Type == BulletType.Character));
// Demonstrate setting the Character property (read-write)
bulletValue.Character = '•';
Console.WriteLine("Bullet Character: " + bulletValue.Character);
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
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
