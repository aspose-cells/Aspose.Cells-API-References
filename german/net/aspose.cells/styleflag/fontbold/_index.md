---
title: "StyleFlag.FontBold"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Fettschrift-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Die Einstellung für fette Schrift wird angewendet.

```csharp
public bool FontBold { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen fetten Stil
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Wende fetten Stil auf Zeile 2 mit StyleFlag nur für Fettschrift an
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Setze einen Wert in die Zelle, um den Stil zu demonstrieren
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


