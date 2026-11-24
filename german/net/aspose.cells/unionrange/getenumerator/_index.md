---
title: "UnionRange.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Gibt den Enumerator für Zellen in diesem Bereich zurück"
type: docs
url: /de/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Ruft den Enumerator für Zellen in diesem Range ab.

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Zellen-Enumerator

### Hinweise

Beim Durchlaufen von Elementen mit dem zurückgegebenen Enumerator sollte die Zellen-Sammlung nicht verändert werden (z. B. Vorgänge, die dazu führen, dass neue Cell/Row instanziiert oder vorhandene Cell/Row gelöscht werden). Andernfalls kann der Enumerator möglicherweise nicht alle Zellen korrekt durchlaufen (einige Elemente könnten mehrfach durchlaufen oder übersprungen werden).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle den ersten Bereich (A1:B2) und fülle ihn mit Daten
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Erstelle den zweiten Bereich (C1:D2) und fülle ihn mit Daten
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Erstelle einen UnionRange aus dem ersten Bereich
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Füge den zweiten Bereich zur Union hinzu
                unionRange = unionRange.Union("C1:D2");

                // Erhalte den Enumerator und iteriere über alle Zellen in der Union
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Speichere die Arbeitsmappe (optional, nur um zu zeigen, dass die Daten erhalten bleiben)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


