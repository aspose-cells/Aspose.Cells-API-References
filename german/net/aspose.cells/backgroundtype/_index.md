---
title: "Enum BackgroundType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.BackgroundType enum. Enumeriert Zellhintergrund-Mustertypen"
type: docs
url: /de/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Enumeriert Zellhintergrundmuster‑Typen.

```csharp
public enum BackgroundType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Stellt ein diagonales Kreuzschraffurmuster dar. |
| DiagonalStripe | `8` | Stellt ein diagonales Streifenmuster dar. |
| Gray6 | `18` | Stellt ein 6,25% Graumuster dar |
| Gray12 | `17` | Stellt ein 12,5% Graumuster dar |
| Gray25 | `4` | Stellt ein 25% Graumuster dar. |
| Gray50 | `2` | Stellt ein 50% Graumuster dar. |
| Gray75 | `3` | Stellt ein 75% Graumuster dar. |
| HorizontalStripe | `5` | Stellt ein horizontales Streifenmuster dar. |
| None | `0` | Stellt keinen Hintergrund dar. |
| ReverseDiagonalStripe | `7` | Stellt ein umgekehrtes diagonales Streifenmuster dar. |
| Solid | `1` | Stellt ein einfarbiges Muster dar. |
| ThickDiagonalCrosshatch | `10` | Stellt ein dickes diagonales Kreuzschraffurmuster dar. |
| ThinDiagonalCrosshatch | `16` | Stellt ein dünnes diagonales Kreuzschraffurmuster dar. |
| ThinDiagonalStripe | `14` | Stellt ein dünnes diagonales Streifenmuster dar. |
| ThinHorizontalCrosshatch | `15` | Stellt ein dünnes horizontales Kreuzschraffurmuster dar. |
| ThinHorizontalStripe | `11` | Stellt ein dünnes horizontales Streifenmuster dar. |
| ThinReverseDiagonalStripe | `13` | Stellt ein dünnes umgekehrtes diagonales Streifenmuster dar. |
| ThinVerticalStripe | `12` | Stellt ein dünnes vertikales Streifenmuster dar. |
| VerticalStripe | `6` | Stellt ein vertikales Streifenmuster dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt in der Arbeitsmappe zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf eine Zelle aus dem Arbeitsblatt zu
            Cell cell = worksheet.Cells["A1"];
            
            // Setzen Sie den Wert der Zelle
            cell.PutValue("Hello, Aspose!");

            // Erstellen Sie ein Stilobjekt
            Style style = cell.GetStyle();
            
            // Legen Sie den Hintergrundmuster-Typ fest
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Legen Sie die Vordergrundfarbe fest
            style.ForegroundColor = Color.Red;
            
            // Legen Sie die Hintergrundfarbe fest
            style.BackgroundColor = Color.Green;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


