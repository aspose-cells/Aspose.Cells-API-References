---
title: "Class CustomFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CustomFilter. Rappresenta il filtro personalizzato"
type: docs
url: /it/net/aspose.cells/customfilter/
---
## CustomFilter class

Rappresenta il filtro personalizzato.

```csharp
public class CustomFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Ottiene e imposta i criteri. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Ottiene e imposta il tipo di operatore del filtro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Imposta i criteri del filtro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Applica il filtro automatico all'intervallo
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Applica un filtro personalizzato per ottenere un'istanza di CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Ottieni il primo filtro personalizzato dalla collezione di filtri
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Visualizza le proprietà del filtro
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Modifica i criteri del filtro usando il metodo SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Visualizza le proprietà del filtro aggiornate
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Salva la cartella di lavoro
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


