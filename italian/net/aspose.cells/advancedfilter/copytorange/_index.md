---
title: "AdvancedFilter.CopyToRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AdvancedFilter. Restituisce l'intervallo in cui copiare il risultato di questo filtro avanzato"
type: docs
url: /it/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Ottiene l'intervallo dove copiare il risultato di questo filtro avanzato.

```csharp
public string CopyToRange { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Aggiungi intervallo dei criteri
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Ottieni l'istanza AdvancedFilter dal foglio di lavoro
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Visualizza il valore della proprietà CopyToRange
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Salva la cartella di lavoro
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


