---
title: "FilterColumn.DynamicFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn‑Eigenschaft. Gibt DynamicFilter zum Filtern mit dynamischen Kriterien zurück"
type: docs
url: /de/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Gibt `DynamicFilter` zum Filtern mit dynamischen Kriterien zurück.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Hinweise

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [`FilterType`](../filtertype/) DynamicFilter ist, andernfalls wird null zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten hinzu
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Auto-Filter anwenden
                worksheet.AutoFilter.Range = "A1:A4";

                // Ermitteln Sie die Filterspalte
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Zugriff auf die DynamicFilter-Eigenschaft (nur lesbar)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // DynamicFilter-Eigenschaften anzeigen
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


