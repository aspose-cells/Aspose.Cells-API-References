---
title: "Metered.GetConsumptionCredit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Metered-Methode. Ruft das Verbrauchsguthaben ab"
type: docs
url: /de/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Verbrauchsguthaben abrufen

```csharp
public static decimal GetConsumptionCredit()
```

### Rückgabewert

Verbrauchsmenge

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz der Metered-Klasse
            Metered metered = new Metered();

            try
            {
                // Rufe die GetConsumptionCredit-Methode statisch auf
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Ergebnis anzeigen
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Erstelle eine einfache Arbeitsmappe, um die Wirkung zu demonstrieren (obwohl GetConsumptionCredit die Arbeitsmappe nicht verändert)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Füge die Verbrauchsguthaben-Informationen zum Arbeitsblatt hinzu
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


