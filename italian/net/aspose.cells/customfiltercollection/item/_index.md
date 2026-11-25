---
title: "CustomFilterCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomFilterCollection. Ottiene il filtro personalizzato nell'indice specifico"
type: docs
url: /it/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Ottiene il filtro personalizzato nell'indice specifico.

```csharp
public CustomFilter this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Crea una nuova CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Accedi alla proprietà Item (sola lettura) usando l'indicizzatore
                // Poiché la collezione è vuota, dimostreremo solo l'accesso alla proprietà
                // In uno scenario reale, dovresti prima aggiungere i filtri tramite altri metodi
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Salva la cartella di lavoro
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


