---
title: "StyleFlag.StyleFlag"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Konstruktor. Erstellt ein Objekt, bei dem alle Flags false sind"
type: docs
url: /de/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Konstruiert ein Objekt, bei dem alle Flags auf false gesetzt sind.

```csharp
public StyleFlag()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen fetten Stil
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Wenden Sie den Stil auf Zeile 9 mit dem StyleFlag-Konstruktor an
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Legen Sie einen Wert in die Zelle und überprüfen Sie den Stil
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


