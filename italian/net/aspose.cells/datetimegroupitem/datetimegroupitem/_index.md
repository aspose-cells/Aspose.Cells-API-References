---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DateTimeGroupItem."
type: docs
url: /it/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| anno | Int32 |  |
| mese | Int32 |  |
| giorno | Int32 |  |
| ora | Int32 |  |
| minuto | Int32 |  |
| secondo | Int32 |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati datetime di esempio alla colonna A
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // Applica l'autofiltro alla colonna delle date
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // Crea un DateTimeGroupItem per il raggruppamento di marzo 2023
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Configura il filtro per mostrare le date di marzo 2023
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Aggiorna il filtro per applicare le modifiche
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Salva la cartella di lavoro filtrata
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


