---
title: "Font.ScriptOffset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Liest und schreibt den Skriptversatz in Prozent."
type: docs
url: /de/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Liest und setzt den Skriptversatz, in Prozent.

```csharp
public double ScriptOffset { get; set; }
```

### Hinweise

Nur für Formen und Diagramme.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze ihren Wert
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Hole den Stil und die Schriftart der Zelle.
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Setze ScriptOffset, um den Subscript/Superscript-Effekt zu demonstrieren.
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Wende den modifizierten Stil wieder auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Überprüfe den ScriptOffset-Wert.
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


