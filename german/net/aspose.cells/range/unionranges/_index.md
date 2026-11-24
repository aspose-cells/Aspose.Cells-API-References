---
title: "Range.UnionRanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt das Union-Ergebnis von zwei Bereichen zurück"
type: docs
url: /de/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Gibt das Ergebnis der Vereinigung von zwei Bereichen zurück.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereiche | Range[] | Der Bereich |

### Rückgabewert

Die Union von zwei Bereichen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in Zellen erstellen
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Bereiche zum Vereinen erstellen
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Rufen Sie UnionRanges mit dem Parameter Range[] auf
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Stil anwenden, um den Vereinigungsbereich anzuzeigen
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


