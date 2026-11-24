---
title: "PivotTable.PivotFilters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt alle Filter in der Pivot-Tabelle zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Gibt alle Filter in der PivotTable zurück.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Erstelle eine Pivot-Tabelle
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Füge Felder zur Pivot-Tabelle hinzu
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Greife auf die PivotFilters-Sammlung zu (schreibgeschützte Eigenschaft)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Zeige Informationen über die PivotFilters-Sammlung an
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Iteriere über die Filter und zeige deren Typen an
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Füge einen Beispiel-Filter hinzu, um die Funktionalität zu demonstrieren
                if (pivotFilters.Count == 0)
                {
                    // Füge dem ersten Feld (Sales) einen Wertefilter hinzu
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Zeige die aktualisierte Filteranzahl an
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Speichere die Arbeitsmappe
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
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

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


