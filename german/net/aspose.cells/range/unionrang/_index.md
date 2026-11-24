---
title: "Range.UnionRang"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt das Union-Ergebnis von zwei Bereichen zurück"
type: docs
url: /de/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Gibt das Ergebnis der Vereinigung von zwei Bereichen zurück.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der Bereich |

### Rückgabewert

Die Union von zwei Bereichen.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode Range.UnionRanges(). Diese Methode wird 12 Monate später, seit Mai 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei Bereiche, um UnionRang zu demonstrieren
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Setze einige Werte in den Bereichen zur Visualisierung
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Rufe die UnionRang-Methode auf, um die beiden Bereiche zu kombinieren
                Range[] unionResult = range1.UnionRang(range2);

                // Zeige Informationen über das Union-Ergebnis an
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Markiere die Union-Bereiche mit einem Rahmen zur Visualisierung
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


