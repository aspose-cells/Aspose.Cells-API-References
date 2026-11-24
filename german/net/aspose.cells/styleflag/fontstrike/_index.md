---
title: "StyleFlag.FontStrike"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung für Durchgestrichen wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Die Einstellung für durchgestrichene Schrift wird angewendet.

```csharp
public bool FontStrike { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Erstelle ein Stil-Objekt und setze FontStrike auf true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Erstelle ein Stil-Flag und aktiviere das FontStrike-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Den Stil mit dem StyleFlag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Zeige den aktuellen FontStrike-Status an
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Erstelle eine weitere Zelle, um Text ohne Durchstreichung zu demonstrieren
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


