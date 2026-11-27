---
title: "Enum SortOnType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SortOnType-enum. Sorterad värdetyp"
type: docs
url: /sv/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Sorterad värdetyp.

```csharp
public enum SortOnType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Value | `0` | Sorterar efter cellernas värde. |
| CellColor | `1` | Sorterar efter cellernas färg. |
| FontColor | `2` | Sorterar efter cellernas teckensnittsfärg. |
| Icon | `3` | Sorterar efter villkorlig ikon. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Applicera autofilter på intervallet
            worksheet.AutoFilter.Range = "A1:B4";

            // Hämta autofiltret
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Hämta datasortering
            DataSorter sorter = autoFilter.Sorter;

            // Ställ in den första nyckeln för att sortera efter värdena i den andra kolumnen (Score)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Sortera data i intervallet
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Spara arbetsboken
            workbook.Save("SortOnTypeExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


