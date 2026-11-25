---
title: "FilterColumn.CustomFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene CustomFilterCollection per filtrare i dati secondo criteri personalizzati"
type: docs
url: /it/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Ottiene [`CustomFilterCollection`](../../customfiltercollection/) per filtrare i dati secondo criteri personalizzati.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Osservazioni

NOTA: Questo setter di questa proprietà è ora obsoleto. Invece, utilizza la proprietà [`FilterType`](../filtertype/) impostandola su CustomFilters. Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Applica filtro automatico
                worksheet.AutoFilter.Range = "A1:A6";

                // Ottieni la colonna del filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Crea e imposta filtri personalizzati usando il metodo AutoFilter.Custom
                // Primo filtro: inizia con "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Secondo filtro: termina con "y" (relazione AND)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Ottieni i filtri personalizzati dalla colonna del filtro
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Visualizza le informazioni dei filtri personalizzati
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Nota: CustomFilterCollection non espone i filtri individuali direttamente
                // attraverso un indicizzatore, quindi possiamo visualizzare solo le proprietà della collezione
                Console.WriteLine("Custom filters have been applied to the column.");

                // Salva la cartella di lavoro
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


