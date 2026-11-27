---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem‑konstruktor."
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | DateTimeGroupingType |  |
| år | Int32 |  |
| månad | Int32 |  |
| dag | Int32 |  |
| timme | Int32 |  |
| minut | Int32 |  |
| sekund | Int32 |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempel på datum-tid-data i kolumn A
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // Applicera autofilter på datumkolumnen
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // Skapa DateTimeGroupItem för mars 2023-gruppering
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Konfigurera filter för att visa mars 2023-datum
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Uppdatera filter för att tillämpa ändringar
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Spara den filtrerade arbetsboken
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


