---
title: "Fill.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Fill-Methode. /"
type: docs
url: /de/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Rufen Sie das FillFormat-Objekt aus der Form ab
                FillFormat fillFormat1 = rectangle.Fill;

                // Erstellen Sie eine weitere Form, um ein zweites FillFormat-Objekt zu erhalten
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Rufen Sie die Equals-Methode auf, um die beiden FillFormat-Objekte zu vergleichen
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Zeigen Sie das Ergebnis des Vergleichs an
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Demonstrieren Sie außerdem den Vergleich mit null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Speichere die Arbeitsmappe
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


