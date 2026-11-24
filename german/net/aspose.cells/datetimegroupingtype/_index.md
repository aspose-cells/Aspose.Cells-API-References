---
title: "Enum DateTimeGroupingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DateTimeGroupingType enum. Gibt an, wie Datum‑Uhrzeit‑Werte gruppiert werden"
type: docs
url: /de/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Gibt an, wie DateTime‑Werte gruppiert werden.

```csharp
public enum DateTimeGroupingType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Day | `0` | Nach Tag gruppieren. |
| Hour | `1` | Nach Stunde gruppieren. |
| Minute | `2` | Nach Minute gruppieren. |
| Month | `3` | Nach Monat gruppieren. |
| Second | `4` | Nach Sekunde gruppieren. |
| Year | `5` | Nach Jahr gruppieren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Erstellen einer Arbeitsmappe und Zugriff auf das erste Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hinzufügen einiger Beispieldaten
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Erstellen eines AutoFilters und Festlegen des Bereichs
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Hinzufügen von Datumsfiltern mit verschiedenen DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Speichern der Arbeitsmappe
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


