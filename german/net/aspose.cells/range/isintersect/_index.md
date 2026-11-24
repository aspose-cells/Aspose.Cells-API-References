---
title: "Range.IsIntersect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt an, ob der Bereich sich überschneidet"
type: docs
url: /de/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Gibt an, ob der Bereich sich schneidet.

```csharp
public bool IsIntersect(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der Bereich. |

### Rückgabewert

Ob der Bereich sich überschneidet.

### Hinweise

Wenn die beiden Bereiche nicht im selben Arbeitsblatt liegen, wird false zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zwei Bereiche, um die Überschneidung zu testen
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // Prüfe, ob range1 mit range2 überschneidet (sollte überschneiden)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // Prüfen Sie, ob range1 mit range3 überschneidet (sollte nicht überschneiden)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Füllen Sie die Bereiche mit verschiedenen Farben, um sie zu visualisieren
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


