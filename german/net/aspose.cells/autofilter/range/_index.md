---
title: "AutoFilter.Range"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Eigenschaft. Gibt den Bereich an, auf den der angegebene AutoFilter angewendet wird"
type: docs
url: /de/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird.

```csharp
public string Range { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Auto-Filter auf den Bereich A1:A5 anwenden
            sheet.AutoFilter.Range = "A1:A5";

            // Den Auto-Filter-Bereich anzeigen
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


