---
title: "Metered.GetConsumptionQuantity"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Metered. Ottiene la dimensione del file di consumo"
type: docs
url: /it/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Ottiene la dimensione del file di consumo

```csharp
public static decimal GetConsumptionQuantity()
```

### Valore di ritorno

quantità di consumo

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Crea un'istanza metered
            Metered metered = new Metered();

            try
            {
                // Imposta le chiavi a consumo (sostituisci con le chiavi reali in uso effettivo)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Ottieni la quantità di consumo
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Visualizza il risultato
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Crea una cartella di lavoro per dimostrare l'uso a consumo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Aggiungi alcuni dati per mostrare che la cartella di lavoro è funzionale
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Salva la cartella di lavoro
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


