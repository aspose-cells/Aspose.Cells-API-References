---
title: "Classe AdvancedFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AdvancedFilter. Rappresenta le impostazioni del filtro avanzato"
type: docs
url: /it/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Rappresenta le impostazioni del filtro avanzato.

```csharp
public class AdvancedFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Ottiene l'intervallo dove copiare il risultato di questo filtro avanzato. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Ottiene l'intervallo dei criteri di questo filtro avanzato. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Ottiene l'intervallo dell'elenco di questo filtro avanzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Popola dati di esempio per l'intervallo dell'elenco
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Popola l'intervallo dei criteri
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Ottieni l'istanza AdvancedFilter dal foglio di lavoro
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Visualizza le proprietà di sola lettura
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Salva la cartella di lavoro
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


