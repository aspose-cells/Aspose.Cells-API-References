---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Metered-Methode. Gibt die Verbrauchsdateigröße zurück"
type: docs
url: /de/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Verbrauchsdateigröße abrufen

```csharp
public static decimal GetConsumptionQuantity()
```

### Rückgabewert

Verbrauchsmenge

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Erstelle eine nutzungsbasierte Instanz
            Metered metered = new Metered();

            try
            {
                // Setze nutzungsbasierte Schlüssel (ersetze durch echte Schlüssel bei realer Nutzung)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Abrufen der Verbrauchsmenge
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Ergebnis anzeigen
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Erstelle ein Arbeitsbuch, um die nutzungsbasierte Nutzung zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Füge einige Daten hinzu, um zu zeigen, dass das Arbeitsbuch funktionsfähig ist
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


