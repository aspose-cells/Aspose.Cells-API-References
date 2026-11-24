---
title: "Klasse DynamicFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DynamicFilter Klasse. Stellt den dynamischen Filter dar"
type: docs
url: /de/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Stellt den dynamischen Filter dar.

```csharp
public class DynamicFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Liest und setzt den Typ dieses dynamischen Filters. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Liest und setzt den Maximalwert des dynamischen Filters. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Liest und setzt den Wert des dynamischen Filters. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Arbeitsmappe und ein Arbeitsblatt (optional für den Kontext)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Fülle einige Beispiel‑numerische Daten ein.
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Definiere einen Autofilter‑Bereich
                worksheet.AutoFilter.Range = "A1:A6";

                // Wende einen dynamischen Filter (AboveAverage) auf die erste Spalte an
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Rufe die von AutoFilter erstellte DynamicFilter‑Instanz ab
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Setze zusätzliche Eigenschaften, falls gewünscht
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Zeige die gesetzten Eigenschaften an
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Aktualisiere den Filter, um Änderungen anzuwenden
                worksheet.AutoFilter.Refresh();

                // Speichere die Arbeitsmappe (die gefilterten Daten werden gespeichert)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


