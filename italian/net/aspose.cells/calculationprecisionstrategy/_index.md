---
title: "Enum CalculationPrecisionStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CalculationPrecisionStrategy enum. Elenca le strategie per gestire la precisione dei calcoli. A causa del problema di precisione dell'aritmetica a virgola mobile IEEE 754, alcune formule apparentemente semplici potrebbero non essere calcolate con il risultato atteso. Come la formula 0.450.430.02, quando si calcolano gli operandi con l'operatore direttamente, il risultato non è zero. Per questo tipo di problema di precisione alcune strategie speciali possono fornire il risultato atteso"
type: docs
url: /it/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Enumera le strategie per gestire la precisione dei calcoli. A causa del problema di precisione dell'aritmetica floating-point IEEE 754, alcune formule "seemingly simple" potrebbero non essere calcolate come il risultato atteso. Ad esempio la formula "=-0.45+0.43+0.02", calcolando gli operandi con l'operatore '+' direttamente, il risultato non è zero. Per questo tipo di problema di precisione, alcune strategie speciali possono fornire il risultato atteso.

```csharp
public enum CalculationPrecisionStrategy
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna strategia applicata al calcolo. Durante il calcolo utilizza semplicemente il valore double originale come operando e restituisce direttamente il risultato. La più efficiente per le prestazioni e applicabile nella maggior parte dei casi. |
| Round | `1` | Arrotonda il risultato del calcolo secondo le cifre significative. |
| Decimal | `2` | Utilizza i decimali come operandi quando possibile. La più inefficiente per le prestazioni. |

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Imposta le opzioni di calcolo
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Calcola le formule nel foglio di lavoro
            workbook.CalculateFormula(calcOptions);

            // Ottieni il risultato della formula
            double result = worksheet.Cells["A2"].DoubleValue;

            // Restituisci il risultato
            Console.WriteLine("Calculated Result: " + result);

            // Salva la cartella di lavoro
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


