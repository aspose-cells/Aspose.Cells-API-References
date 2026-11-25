---
title: "PivotTable.PivotFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce tutti i filtri nella tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Restituisce tutti i filtri nella tabella pivot.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
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
                // Crea una tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Aggiungi campi alla tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Accedi alla collezione PivotFilters (proprietà di sola lettura)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Visualizza le informazioni sulla collezione PivotFilters
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Itera attraverso i filtri e visualizza i loro tipi
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Aggiungi un filtro di esempio per dimostrare la funzionalità
                if (pivotFilters.Count == 0)
                {
                    // Aggiungi un filtro di valore al primo campo (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Visualizza il conteggio aggiornato dei filtri
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


