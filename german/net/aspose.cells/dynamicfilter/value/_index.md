---
title: "DynamicFilter.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DynamicFilter-Eigenschaft. Liest und schreibt den dynamischen Filterwert"
type: docs
url: /de/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Liest und setzt den Wert des dynamischen Filters.

```csharp
public object Value { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Zeige den aktuellen Filterwert
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Ändere den Filterwert, um Aprildaten anzuzeigen
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Filter anwenden
            worksheet.AutoFilter.Refresh();

            // Ergebnis speichern
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


