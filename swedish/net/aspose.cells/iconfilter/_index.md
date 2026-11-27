---
title: "Klass IconFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IconFilter-klass. Representerar ikonfilter"
type: docs
url: /sv/net/aspose.cells/iconfilter/
---
## IconFilter class

Representerar ikonfilter.

```csharp
public class IconFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Hämtar och anger nollbaserat index för en ikon i en ikonuppsättning. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Hämtar och anger vilken ikonuppsättning som används för detta filterkriterium. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fyll i exempeldata
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Skapa autofilter
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Hämta ikonfiltret
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Ställ in ikonfilteregenskaper
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Spara arbetsboken
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


