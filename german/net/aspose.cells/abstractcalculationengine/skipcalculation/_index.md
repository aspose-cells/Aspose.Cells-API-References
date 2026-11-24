---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationEngine-Methode. Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert."
type: docs
url: /de/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert.

```csharp
public void SkipCalculation()
```

### Hinweise

Diese Methode kann in der Implementierung von [`Calculate`](../calculate/) aufgerufen werden, um die Berechnung der gesamten Formel zu überspringen, wobei der ursprüngliche Wert der Formel unverändert bleibt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Erstelle eine benutzerdefinierte Berechnungs-Engine
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Berechne die Arbeitsmappe, die unsere benutzerdefinierte Engine auslöst
                workbook.CalculateFormula(options);

                // Zeige das Ergebnis an (sollte übersprungen werden)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Speichere die Arbeitsmappe
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Überspringe die Berechnung für diese Formel
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


