---
title: "Enum MsoArrowheadStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoArrowheadStyle Enum. Enumeriert den Linientyp des Endes der Formkontur"
type: docs
url: /de/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumeriert den Endtyp der Linien des Formrahmens.

```csharp
public enum MsoArrowheadStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Linientyp. |
| Arrow | `1` | Pfeil-Linientyp. |
| ArrowStealth | `2` | Pfeil‑Stealth-Linientyp. |
| ArrowDiamond | `3` | Pfeil-Diamant-Linienendtyp. |
| ArrowOval | `4` | Pfeil-Oval-Linienendtyp. |
| ArrowOpen | `5` | Pfeil-Offen-Linienendtyp. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Linieneigenschaften festlegen
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Pfeilspitzenstile festlegen
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


