---
title: "Enum ShapeLockType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeLockType-enum. Representerar typen av egenskapen som ska låsas"
type: docs
url: /sv/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Representerar typen av egenskapen som ska låsas.

```csharp
public enum ShapeLockType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Group | `0` | Grupp |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Text |
| Points | `3` | Punkter |
| Crop | `4` | Beskär |
| Selection | `5` | Markering |
| Move | `6` | Flytta |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Avgruppera |
| Resize | `10` | Ändra storlek |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Pilspets |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Demonstrera funktionaliteten för ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


