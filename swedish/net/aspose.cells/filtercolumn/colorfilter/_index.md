---
title: "FilterColumn.ColorFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskap. Hämtar ColorFilter för att filtrera data efter färg"
type: docs
url: /sv/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Hämtar [`ColorFilter`](../../colorfilter/) för att filtrera data efter färg.

```csharp
public ColorFilter ColorFilter { get; }
```

### Anmärkningar

Sätter [`FilterType`](../filtertype/) till ColorFilter först, annars returneras Null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata med färger
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Applicera autofilter
                worksheet.AutoFilter.Range = "A1:A4";

                // Hämta filterkolumnen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Åtkomst till ColorFilter-egenskapen (endast läsning)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Visa ColorFilter-egenskaper
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Spara arbetsboken
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


