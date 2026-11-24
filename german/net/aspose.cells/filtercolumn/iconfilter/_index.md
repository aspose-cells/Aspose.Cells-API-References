---
title: "FilterColumn.IconFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn‑Eigenschaft. Gibt IconFilter zum Filtern von Daten nach Symbol zurück"
type: docs
url: /de/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Gibt `IconFilter` zum Filtern von Daten nach Symbol zurück.

```csharp
public IconFilter IconFilter { get; }
```

### Hinweise

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [`FilterType`](../filtertype/) IconFilter ist, andernfalls wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten mit bedingter Formatierung hinzu, die Symbole nutzt
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Wende Auto-Filter auf den Bereich an
                worksheet.AutoFilter.Range = "A1:A5";

                // Ermitteln Sie die Filterspalte
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Zugriff auf die IconFilter‑Eigenschaft (schreibgeschützt)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Zeigen Sie die IconFilter‑Eigenschaften an, falls sie vorhanden sind
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


