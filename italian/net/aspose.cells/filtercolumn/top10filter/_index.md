---
title: "FilterColumn.Top10Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene Top10Filter per filtrare i dati in base al rango dei dati"
type: docs
url: /it/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Ottiene `Top10Filter` per filtrare i dati in base al rango dei dati.

```csharp
public Top10Filter Top10Filter { get; }
```

### Osservazioni

Prima di utilizzare questa proprietà, assicurati che [`FilterType`](../filtertype/) sia Top10, altrimenti verrà restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Popola alcuni dati di esempio
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Applica un AutoFilter all'intervallo di dati
                sheet.AutoFilter.Range = "A1:A5";

                // Ottieni la prima colonna del filtro (indice colonna 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Visualizza l'oggetto Filter corrente (potrebbe essere null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Verifica se il filtro applicato è un Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


