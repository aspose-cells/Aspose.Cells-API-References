---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractCalculationEngine. Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione"
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione.

```csharp
public void SkipCalculation()
```

### Osservazioni

Questo metodo può essere invocato nell'implementazione di [`Calculate`](../calculate/) per saltare il calcolo per l'intera formula e il valore originale della formula verrà mantenuto senza modifiche.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Crea un motore di calcolo personalizzato
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Calcola la cartella di lavoro che attiverà il nostro motore personalizzato
                workbook.CalculateFormula(options);

                // Visualizza il risultato (dovrebbe essere saltato)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Salva la cartella di lavoro
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
                // Salta il calcolo per questa formula
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


