---
title: "StyleFlag.LeftBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellungen für den linken Rand werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Die Einstellungen für den linken Rand werden angewendet.

```csharp
public bool LeftBorder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich und wende den linken Randstil an
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Erstelle Stil und Flag
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Setze die Eigenschaften des linken Randes
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Wende den Stil mit dem linken Rand-Flag an
            range.ApplyStyle(style, flag);

            // Überprüfe, ob der linke Rand angewendet wurde
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Speichere die Arbeitsmappe
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


