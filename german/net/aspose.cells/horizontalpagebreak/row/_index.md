---
title: "HorizontalPageBreak.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HorizontalPageBreak-Eigenschaft. Gibt den nullbasierten Zeilenindex zurück"
type: docs
url: /de/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Gibt den nullbasierten Zeilenindex zurück.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge horizontale Seitenumbrüche hinzu
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Abrufen der Sammlung horizontaler Seitenumbrüche
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Zeige Zeilennummern der Seitenumbrüche
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


