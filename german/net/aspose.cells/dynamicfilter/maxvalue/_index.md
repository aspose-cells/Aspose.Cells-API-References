---
title: "DynamicFilter.MaxValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DynamicFilter-Eigenschaft. Liest und schreibt den maximalen dynamischen Filterwert"
type: docs
url: /de/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Liest und setzt den Maximalwert des dynamischen Filters.

```csharp
public object MaxValue { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispielzahlen hinzu
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Wende dynamischen Filter mit Bereichskriterien an
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Zeige den aktuellen MaxValue
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Da DynamicFilterType.Between nicht existiert, verwenden wir einen anderen Ansatz
            // Zum Beispiel können wir stattdessen einen benutzerdefinierten Filter verwenden
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Filter anwenden
            worksheet.AutoFilter.Refresh();

            // Ergebnis speichern
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


