---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Konstruktor."
type: docs
url: /de/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | DateTimeGroupingType |  |
| Jahr | Int32 |  |
| Monat | Int32 |  |
| Tag | Int32 |  |
| Stunde | Int32 |  |
| Minute | Int32 |  |
| Sekunde | Int32 |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Datum/Uhrzeit zu Spalte A hinzufügen
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // AutoFilter auf die Datumsspalte anwenden
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // DateTimeGroupItem für die Gruppierung im März 2023 erstellen
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Filter konfigurieren, um Daten aus März 2023 anzuzeigen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Filter aktualisieren, um Änderungen anzuwenden
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Die gefilterte Arbeitsmappe speichern
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


