---
title: "UnionRange.Hyperlinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt alle Hyperlinks im Bereich zurück"
type: docs
url: /de/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Liefert alle Hyperlinks im Bereich.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Hyperlinks zu Zellen hinzu
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Erstelle einen Bereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Erhalte Hyperlinks im Bereich
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Zeige Informationen zu jedem Hyperlink an
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


