---
title: "CellsHelper.GetTextWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper method. Ermittelt die Breite des Textes in der Einheit Punkte."
type: docs
url: /de/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Ermittelt die Breite des Textes in Punkt.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text. |
| Schriftart | Schriftart | Die Schriftart des Textes. |
| Skalierung | Double | Die Skalierung des Textes. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


