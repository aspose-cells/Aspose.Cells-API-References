---
title: "Style.Pattern"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt den Hintergrundmuster-Typ einer Zelle zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Liest oder setzt den Hintergrundmuster-Typ der Zelle.

```csharp
public BackgroundType Pattern { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Greife auf die Zelle zu und erhalte ihren Stil
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Setze Muster und Vordergrundfarbe
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


