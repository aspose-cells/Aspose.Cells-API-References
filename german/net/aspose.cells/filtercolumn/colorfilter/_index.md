---
title: "FilterColumn.ColorFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn‑Eigenschaft. Gibt ColorFilter zum Filtern von Daten nach Farbe zurück"
type: docs
url: /de/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Gibt [`ColorFilter`](../../colorfilter/) zum Filtern von Daten nach Farbe zurück.

```csharp
public ColorFilter ColorFilter { get; }
```

### Hinweise

Setzt [`FilterType`](../filtertype/) zuerst auf ColorFilter, andernfalls wird Null zurückgegeben.

### Beispiele

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
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Beispieldaten mit Farben hinzufügen
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Auto-Filter anwenden
                worksheet.AutoFilter.Range = "A1:A4";

                // Ermitteln Sie die Filterspalte
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Zugriff auf die ColorFilter‑Eigenschaft (schreibgeschützt)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // ColorFilter‑Eigenschaften anzeigen
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


