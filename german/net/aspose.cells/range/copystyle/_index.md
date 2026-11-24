---
title: "Range.CopyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Kopiert Stileinstellungen von einem Quell-Range"
type: docs
url: /de/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Kopiert Stil­einstellungen aus einem Quellbereich.

```csharp
public void CopyStyle(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | Range | Quell-[`Range`](../) Objekt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Füge dem Quell-Range einen Beispielstil hinzu
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Erstelle ein Ziel-Arbeitsblatt
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Erstelle einen Ziel-Range und kopiere den Stil
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


