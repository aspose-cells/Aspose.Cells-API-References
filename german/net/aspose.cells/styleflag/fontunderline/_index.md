---
title: "StyleFlag.FontUnderline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung der Schriftunterstreichung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Die Einstellung für unterstrichene Schrift wird angewendet.

```csharp
public bool FontUnderline { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Ein Stilobjekt erstellen und Schriftunterstreichung festlegen
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Ein StyleFlag erstellen und das Schriftunterstreichungs-Flag aktivieren
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Den Stil mit dem StyleFlag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Aktuellen Unterstreichungsstatus anzeigen
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Unterstreichungsart auf doppelt ändern
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Speichere die Arbeitsmappe
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


