---
title: "UnionRange.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Kopiert den Bereich mit Spezial-Einfügeoptionen"
type: docs
url: /de/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Kopieren des Bereichs mit Spezial‑Einfügeoptionen.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | UnionRange | Der Quellbereich. |
| Optionen | PasteOptions | Die Spezial-Einfügeoptionen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Erstellen Sie die Quell-UnionRange
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Erstellen Sie die Ziel-UnionRange
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Erstellen Sie PasteOptions mit spezifischen Einstellungen
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Rufen Sie die Copy-Methode auf
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Speichere die Arbeitsmappe
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


