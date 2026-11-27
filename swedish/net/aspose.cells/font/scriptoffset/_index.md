---
title: "Font.ScriptOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar och anger skriptförskjutningen i procentenheter"
type: docs
url: /sv/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Hämtar och anger skriptförskjutningen, i procentenheter

```csharp
public double ScriptOffset { get; set; }
```

### Anmärkningar

Endast för former och diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cell A1 och ange dess värde
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Hämta stil och teckensnitt för cellen
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Ange ScriptOffset för att demonstrera nedsänkt/upphöjt effekt
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Applicera den ändrade stilen tillbaka till cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Verifiera ScriptOffset‑värdet
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


