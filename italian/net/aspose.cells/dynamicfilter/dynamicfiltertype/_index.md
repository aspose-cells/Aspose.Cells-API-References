---
title: "DynamicFilter.DynamicFilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DynamicFilter. Ottiene e imposta il tipo di questo filtro dinamico"
type: docs
url: /it/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Ottiene e imposta il tipo di questo filtro dinamico.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con date
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Crea filtro automatico
                worksheet.AutoFilter.Range = "A1:A5";

                // Applica filtro dinamico per le date di marzo
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Ottieni l'istanza di DynamicFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Visualizza il valore corrente di DynamicFilterType
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Modifica il tipo di filtro per mostrare le date di aprile
                filter.DynamicFilterType = DynamicFilterType.April;

                // Visualizza il valore aggiornato di DynamicFilterType
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Applica il filtro
                worksheet.AutoFilter.Refresh();

                // Salva il risultato
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

### Vedi anche

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


