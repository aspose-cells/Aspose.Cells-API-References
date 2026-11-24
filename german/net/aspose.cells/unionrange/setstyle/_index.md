---
title: "UnionRange.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Legt den Stil des Bereichs fest"
type: docs
url: /de/net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Legt den Stil des Bereichs fest.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Style-Objekt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle einige Beispieldaten in den Bereich A1:B2 ein
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue("Total");
            worksheet.Cells["B2"].PutValue(456);

            // Erstelle einen UnionRange, der die Zellen A1:B2 abdeckt
            UnionRange unionRange = worksheet.Cells
                .CreateRange("A1:B2")
                .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Erstelle eine Style-Instanz und setze einige Formatierungen
                Style style = new Style();
                style.BackgroundColor = Color.LightYellow;
                style.ForegroundColor = Color.DarkBlue;
                style.HorizontalAlignment = TextAlignmentType.Center;
                style.VerticalAlignment = TextAlignmentType.Center;
                style.IsTextWrapped = true;

                // Wende den Stil auf den UnionRange an
                unionRange.SetStyle(style);

                Console.WriteLine("SetStyle executed successfully on the UnionRange.");

                // Speichere die Arbeitsmappe, um das Ergebnis zu visualisieren
                workbook.Save("UnionRangeSetStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetStyle: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


