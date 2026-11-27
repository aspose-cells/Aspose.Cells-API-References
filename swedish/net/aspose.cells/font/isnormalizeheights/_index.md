---
title: "Font.IsNormalizeHeights"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Anger om normalisering av höjd som ska tillämpas på textsekvensen"
type: docs
url: /sv/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Indikerar om normaliseringen av höjden som ska tillämpas på textkörningen.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### Anmärkningar

Endast för teckensnitten i former eller diagram. OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/). Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // Ange egenskapen IsNormalizeHeights
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // Verifiera egenskapen
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // Ändra egenskapen
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


