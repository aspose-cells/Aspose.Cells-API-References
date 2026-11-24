---
title: "AutoFilter.Sorter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter‑Eigenschaft. Gibt den Datensortierer zurück"
type: docs
url: /de/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Liest den Datensortierer.

```csharp
public DataSorter Sorter { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Auto-Filter-Bereich erstellen
            worksheet.AutoFilter.Range = "A1:B4";

            // Hole den Auto-Filter
            AutoFilter filter = worksheet.AutoFilter;

            // Filter anwenden
            filter.Filter(1, "10");

            // Sortieren mit der Sorter‑Eigenschaft
            filter.Sorter.Sort();

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


