---
title: "FilterColumn.MultipleFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene MultipleFilterCollection per filtrare i dati per etichette o data/ora"
type: docs
url: /it/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Ottiene [`MultipleFilterCollection`](../../multiplefiltercollection/) per filtrare i dati per etichette o data/ora.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà FilterColumn.FilterValues. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Applica AutoFilter all'intervallo
                worksheet.AutoFilter.Range = "A1:A5";

                // Ottieni la prima colonna del filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Crea e imposta MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Assegna i MultipleFilters alla colonna filtro
                filterColumn.MultipleFilters = multipleFilters;

                // Visualizza le proprietà dei MultipleFilters
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Salva la cartella di lavoro
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


