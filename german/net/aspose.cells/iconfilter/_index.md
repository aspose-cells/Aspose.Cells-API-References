---
title: "Klasse IconFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IconFilter Klasse. Stellt den Symbolfilter dar"
type: docs
url: /de/net/aspose.cells/iconfilter/
---
## IconFilter class

Stellt einen Symbolfilter dar.

```csharp
public class IconFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Liest und setzt den nullbasierten Index eines Symbols in einem Symbolset. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Liest und setzt, welches Symbolset für dieses Filterkriterium verwendet wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten befüllen
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Automatischen Filter erstellen
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Liest den Symbolfilter
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Icon-Filter-Eigenschaften festlegen
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


