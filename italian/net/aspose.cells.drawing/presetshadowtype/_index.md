---
title: "Enumerazione PresetShadowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enumerazione Aspose.Cells.Drawing.PresetShadowType. Rappresenta il tipo di ombra predefinito"
type: docs
url: /it/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Rappresenta il tipo di ombra predefinito.

```csharp
public enum PresetShadowType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NoShadow | `0` | Nessuna ombra. |
| Custom | `1` | Ombra personalizzata. |
| OffsetDiagonalBottomRight | `2` | Offset dell'ombra esterna diagonale in basso a destra. |
| OffsetBottom | `3` | Offset dell'ombra esterna in basso. |
| OffsetDiagonalBottomLeft | `4` | Ombra esterna offset diagonale in basso a sinistra. |
| OffsetRight | `5` | Ombra esterna offset a destra. |
| OffsetCenter | `6` | Ombra esterna offset al centro. |
| OffsetLeft | `7` | Ombra esterna offset a sinistra. |
| OffsetDiagonalTopRight | `8` | Ombra esterna offset diagonale in alto a destra. |
| OffsetTop | `9` | Ombra esterna offset in alto. |
| OffsetDiagonalTopLeft | `10` | Ombra esterna offset diagonale in alto a sinistra. |
| InsideDiagonalTopLeft | `11` | Ombra interna dentro diagonale in alto a Sinistra. |
| InsideTop | `12` | Ombra interna dentro in alto. |
| InsideDiagonalTopRight | `13` | Ombra interna dentro diagonale in alto a destra. |
| InsideLeft | `14` | Ombra interna dentro a sinistra. |
| InsideCenter | `15` | Ombra interna dentro al centro. |
| InsideRight | `16` | Ombra interna dentro a destra. |
| InsideDiagonalBottomLeft | `17` | Ombra interna dentro diagonale in basso a sinistra. |
| InsideBottom | `18` | Ombra interna dentro in basso. |
| InsideDiagonalBottomRight | `19` | Ombra interna dentro diagonale in basso a destra. |
| PerspectiveDiagonalUpperLeft | `20` | Ombra esterna prospettiva diagonale in alto a sinistra. |
| PerspectiveDiagonalUpperRight | `21` | Ombra esterna prospettiva diagonale in alto a destra. |
| Below | `22` | Ombra esterna sotto. |
| PerspectiveDiagonalLowerLeft | `23` | Ombra esterna prospettiva diagonale in basso a sinistra. |
| PerspectiveDiagonalLowerRight | `24` | Ombra esterna prospettiva diagonale in basso a destra. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare gli effetti di ombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Imposta diversi tipi di ombra predefiniti
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Cambia a un altro tipo di ombra
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Salva la cartella di lavoro
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


