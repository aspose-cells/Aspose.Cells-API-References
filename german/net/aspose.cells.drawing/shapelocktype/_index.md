---
title: "Aufzählung ShapeLockType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapeLockType-Aufzählung. Stellt den Typ der zu sperrenden Eigenschaft dar"
type: docs
url: /de/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Stellt den Typ der zu sperrenden Eigenschaft dar.

```csharp
public enum ShapeLockType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Group | `0` | Gruppe |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Text |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Beispiele

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

            // Ein Bild zum Arbeitsblatt hinzufügen
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Demonstrieren Sie die Funktionalität von ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


