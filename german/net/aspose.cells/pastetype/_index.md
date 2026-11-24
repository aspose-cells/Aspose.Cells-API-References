---
title: "Aufzählung PasteType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PasteType‑Enum. Stellt den Spezial‑Einfügetyp dar."
type: docs
url: /de/net/aspose.cells/pastetype/
---
## PasteType enumeration

Stellt den Spezial-Einfügen-Typ dar.

```csharp
public enum PasteType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `0` | Kopiert alle Daten des Bereichs. |
| Default | `1` | Es funktioniert wie das „All“-Verhalten von MS Excel. |
| AllExceptBorders | `2` | Kopiert alle Daten des Bereichs ohne den Bereich. |
| DefaultExceptBorders | `3` | Es funktioniert wie das „All except borders“-Verhalten von MS Excel. |
| ColumnWidths | `4` | Kopiert nur die Breiten des Bereichs. |
| RowHeights | `5` | Kopiert nur die Höhen des Bereichs. |
| Comments | `6` | Kopiert nur Kommentare im Bereich. |
| Formats | `7` | Kopiert nur Formate im Bereich. |
| Formulas | `8` | Kopiert nur Formeln im Bereich. |
| FormulasAndNumberFormats | `9` | Kopiert nur Formeln und Zahlenformate im Bereich. |
| Validation | `10` | Kopiert nur Validierungen im Bereich. |
| Values | `11` | Kopiert nur Werte im Bereich. |
| ValuesAndFormats | `12` | Kopiert nur Werte und Formate im Bereich. |
| ValuesAndNumberFormats | `13` | Kopiert nur Werte und Zahlenformate im Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Quellbereich definieren
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Zielbereich definieren
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Erstellen Sie PasteOptions und setzen Sie den PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Kopieren Sie den Quellbereich in den Zielbereich mit den angegebenen PasteOptions
            destinationRange.Copy(sourceRange, pasteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("PasteTypeExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


