---
title: "Klasse CustomFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CustomFilter Klasse. Stellt den benutzerdefinierten Filter dar"
type: docs
url: /de/net/aspose.cells/customfilter/
---
## CustomFilter class

Stellt den benutzerdefinierten Filter dar.

```csharp
public class CustomFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Liest und setzt die Kriterien. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Liest und setzt den Filteroperatortyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Setzt die Filterkriterien. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten zum Arbeitsblatt hinzufügen
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Wende Auto-Filter auf den Bereich an
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Wende einen benutzerdefinierten Filter an, um eine CustomFilter-Instanz zu erhalten
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Holen Sie den ersten benutzerdefinierten Filter aus der Filtersammlung
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Zeigen Sie die Filtereigenschaften an
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Ändern Sie die Filterkriterien mit der Methode SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Zeigen Sie die aktualisierten Filtereigenschaften an
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Speichere die Arbeitsmappe
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


