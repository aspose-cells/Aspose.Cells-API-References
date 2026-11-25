---
title: "CustomFilter.SetCriteria"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomFilter. Imposta i criteri del filtro"
type: docs
url: /it/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Imposta i criteri del filtro.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filterOperator | FilterOperatorType | tipo di operatore del filtro |
| criteri | Object | valore dei criteri del filtro |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Applica un filtro personalizzato per ottenere un'istanza di CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Ottieni il primo filtro personalizzato dalla collezione di filtri
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Imposta i criteri usando il metodo SetCriteria
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Mostra i criteri impostati
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Salva la cartella di lavoro
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


