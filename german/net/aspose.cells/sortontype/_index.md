---
title: "Enum SortOnType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SortOnType Enum. Sortierter Werttyp"
type: docs
url: /de/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Sortierter Werttyp.

```csharp
public enum SortOnType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Value | `0` | Sortiert nach dem Zellenwert. |
| CellColor | `1` | Sortiert nach der Zellenfarbe. |
| FontColor | `2` | Sortiert nach der Schriftfarbe der Zellen. |
| Icon | `3` | Sortiert nach dem bedingten Symbol. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
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

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Wende Auto-Filter auf den Bereich an
            worksheet.AutoFilter.Range = "A1:B4";

            // Hole den Auto-Filter
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Hole den Datensortierer
            DataSorter sorter = autoFilter.Sorter;

            // Setze den ersten Schlüssel, um nach den Werten in der zweiten Spalte (Score) zu sortieren
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Sortiere die Daten im Bereich
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("SortOnTypeExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


