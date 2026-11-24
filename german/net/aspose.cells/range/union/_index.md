---
title: "Range.Union"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt die Union von zwei Bereichen zurück"
type: docs
url: /de/net/aspose.cells/range/union/
---
## Range.Union method

Gibt die Union von zwei Bereichen zurück.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der Bereich |

### Rückgabewert

Die Union von zwei Bereichen.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode Range.UnionRanges(). Diese Methode wird 12 Monate später, seit November 2023, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei Bereiche, um Union zu demonstrieren
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Fülle einige Daten in die Bereiche
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Rufe die Union-Methode auf (Hinweis: dies ist die veraltete Version)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Zeige die Adressen aller Bereiche in der Union an
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


