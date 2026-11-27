---
title: "Enum LightRigDirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Representerar typen för ljusriggens riktning"
type: docs
url: /sv/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Representerar ljusriggens riktningstyp.

```csharp
public enum LightRigDirectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Bottom | `0` | Botten |
| BottomLeft | `1` | Nederst till vänster. |
| BottomRight | `2` | Nedre höger. |
| Left | `3` | Vänster. |
| Right | `4` | Höger. |
| Top | `5` | Överst. |
| TopLeft | `6` | Överst till vänster. |
| TopRight | `7` | Övre höger. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera ljusriggens riktning
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Ställ in ljusriggens riktning för formens 3D-format
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Demonstrera olika ljusriggens riktningar
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Ändra ljusriggens riktning
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Iterera genom alla möjliga ljusriggens riktningar
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Spara arbetsboken
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


