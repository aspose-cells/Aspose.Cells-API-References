---
title: "StyleFlag.TextDirection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Textrichtungseinstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Die Einstellung für die Textausrichtung wird angewendet.

```csharp
public bool TextDirection { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Erstelle einen Stil und setze die Textausrichtung
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Erstelle ein Stil-Flag und aktiviere das TextDirection-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Den Stil mit dem StyleFlag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Zeige die aktuelle Textausrichtung an
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Ändere die Textausrichtung und wende sie erneut an
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Speichere die Arbeitsmappe
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


