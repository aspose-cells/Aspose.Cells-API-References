---
title: "DynamicFilter.DynamicFilterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DynamicFilter-Eigenschaft. Liest und schreibt den Typ dieses dynamischen Filters"
type: docs
url: /de/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Liest und setzt den Typ dieses dynamischen Filters.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Datumsangaben hinzufügen
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Automatischen Filter erstellen
                worksheet.AutoFilter.Range = "A1:A5";

                // Wende dynamischen Filter für März-Daten an
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Abrufen der DynamicFilter-Instanz
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Zeige den aktuellen DynamicFilterType-Wert
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Ändere den Filtertyp, um Aprildaten anzuzeigen
                filter.DynamicFilterType = DynamicFilterType.April;

                // Zeige den aktualisierten DynamicFilterType-Wert
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Filter anwenden
                worksheet.AutoFilter.Refresh();

                // Ergebnis speichern
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


