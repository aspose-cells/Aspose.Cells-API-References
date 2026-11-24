---
title: "StyleFlag.FontScript"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung für Schriftartskript wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Die Einstellung für das Schriftskript wird angewendet.

```csharp
public bool FontScript { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Erstelle ein Stil-Objekt und setze das Schriftartskript auf Tiefstellung
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Erstelle ein Stil-Flag und aktiviere das FontScript-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Den Stil mit dem StyleFlag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Zeige den aktuellen Schriftartskript-Status an
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Ändere das Schriftartskript zu Hochstellung
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Zeige den aktualisierten Schriftartskript-Status an
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


