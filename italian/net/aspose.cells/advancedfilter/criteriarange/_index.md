---
title: "AdvancedFilter.CriteriaRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AdvancedFilter. Restituisce l'intervallo dei criteri di questo filtro avanzato"
type: docs
url: /it/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Ottiene l'intervallo dei criteri di questo filtro avanzato.

```csharp
public string CriteriaRange { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Popola dati di esempio per l'intervallo dell'elenco
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Popola i criteri di esempio (il filtro li utilizzerà quando applicato)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Ottieni l'oggetto AdvancedFilter per il foglio di lavoro
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // Le proprietà ListRange, CriteriaRange e CopyToRange sono di sola lettura.
                // Visualizza gli intervalli determinati automaticamente.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Salva la cartella di lavoro (opzionale, solo per mostrare che il file può essere creato)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


