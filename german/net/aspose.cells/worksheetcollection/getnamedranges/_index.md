---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab"
type: docs
url: /de/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab.

```csharp
public Range[] GetNamedRanges()
```

### Rückgabewert

Ein Array von Range-Objekten. Wenn die Referenz des definierten Namens extern ist oder mehrere Bereiche enthält, wird kein Range-Objekt für diesen Namen zurückgegeben.

Gibt null zurück, wenn der benannte Bereich nicht existiert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einige benannte Bereiche zur Demonstration
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Rufe die GetNamedRanges-Methode auf, um alle benannten Bereiche abzurufen
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Zeige Informationen zu den benannten Bereichen an
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Speichere die Arbeitsmappe
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


