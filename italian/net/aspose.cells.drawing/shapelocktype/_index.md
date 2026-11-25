---
title: "Enumerazione ShapeLockType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enumerazione Aspose.Cells.Drawing.ShapeLockType. Rappresenta il tipo della proprietà da bloccare"
type: docs
url: /it/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Rappresenta il tipo della proprietà da bloccare.

```csharp
public enum ShapeLockType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Group | `0` | Gruppo |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Testo |
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

### Esempi

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

            // Aggiungi un'immagine al foglio di lavoro
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Dimostrare la funzionalità di ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


