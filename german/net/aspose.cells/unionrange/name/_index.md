---
title: "UnionRange.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt den Namen des Bereichs zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Liefert oder setzt den Namen des Bereichs.

```csharp
public string Name { get; set; }
```

### Hinweise

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Erstellen Sie Bereiche und kombinieren Sie sie zu einem Union-Bereich
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Zeige den aktuellen Wert der Name-Eigenschaft an
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Setze einen neuen Namen für den UnionRange
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Demonstriere, dass der Name erneut geändert werden kann
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Speichere die Arbeitsmappe
                workbook.Save("UnionRangeNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


