---
title: "FilterColumn.Top10Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn egenskap. Hämtar Top10Filter för filtrering av data efter rangordning"
type: docs
url: /sv/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Hämtar `Top10Filter` för filtrering av data efter rangordning.

```csharp
public Top10Filter Top10Filter { get; }
```

### Anmärkningar

Innan du använder denna egenskap, se till att [`FilterType`](../filtertype/) är Top10, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fyll i lite exempeldata
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Applicera ett AutoFilter på dataområdet
                sheet.AutoFilter.Range = "A1:A5";

                // Hämta den första filterkolumnen (kolumnindex 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Visa det aktuella Filter-objektet (kan vara null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Kontrollera om det tillämpade filtret är ett Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Spara arbetsboken (valfritt)
                workbook.Save("Top10FilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


