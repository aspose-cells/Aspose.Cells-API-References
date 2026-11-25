---
title: "Metered.GetConsumptionCredit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Metered. Ottiene il credito di consumo"
type: docs
url: /it/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Ottiene il credito di consumo

```csharp
public static decimal GetConsumptionCredit()
```

### Valore di ritorno

quantità di consumo

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Crea un'istanza della classe Metered
            Metered metered = new Metered();

            try
            {
                // Chiama il metodo GetConsumptionCredit in modo statico
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Visualizza il risultato
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Crea una semplice cartella di lavoro per dimostrare l'effetto (anche se GetConsumptionCredit non modifica la cartella di lavoro)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Aggiungi le informazioni sul credito di consumo al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Salva la cartella di lavoro
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


