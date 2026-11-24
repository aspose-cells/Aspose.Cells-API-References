---
title: "Worksheet.AutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet property. Stellt den AutoFilter für das angegebene Arbeitsblatt dar."
type: docs
url: /de/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Stellt den AutoFilter für das angegebene Arbeitsblatt dar.

```csharp
public AutoFilter AutoFilter { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Filter aktualisieren
            worksheet.AutoFilter.Refresh();

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


