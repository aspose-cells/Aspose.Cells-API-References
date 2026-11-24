---
title: "Aufzählung CalculationPrecisionStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CalculationPrecisionStrategy-Enum. Enumeriert Strategien zur Handhabung der Berechnungsgenauigkeit. Aufgrund des Präzisionsproblems der IEEE‑754‑Fließkommaarithmetik können scheinbar einfache Formeln nicht das erwartete Ergebnis liefern. Zum Beispiel ergibt die Formel 0.450.430.02 bei direkter Berechnung der Operanden durch den Operator kein Null‑Ergebnis. Für solche Präzisionsprobleme können spezielle Strategien das erwartete Ergebnis liefern."
type: docs
url: /de/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Enumeriert Strategien zum Umgang mit Berechnungspräzision. Aufgrund des Präzisionsproblems der IEEE‑754‑Gleitkommaarithmetik können einige \"scheinbar einfache\" Formeln nicht das erwartete Ergebnis liefern. Zum Beispiel die Formel \"=-0.45+0.43+0.02\", bei direkter Berechnung der Operanden mit dem '+'‑Operator ist das Ergebnis nicht null. Für solche Präzisionsprobleme können einige spezielle Strategien das erwartete Ergebnis liefern.

```csharp
public enum CalculationPrecisionStrategy
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Strategie bei der Berechnung angewendet. Beim Berechnen einfach den ursprünglichen double‑Wert als Operand verwenden und das Ergebnis direkt zurückgeben. Am effizientesten für die Leistung und in den meisten Fällen anwendbar. |
| Round | `1` | Rundet das Berechnungsergebnis gemäß den signifikanten Stellen. |
| Decimal | `2` | Verwendet Dezimalzahlen als Operanden, wenn möglich. Am wenigsten effizient für die Leistung. |

### Beispiele

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Setzen Sie Berechnungsoptionen
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Berechne die Formeln im Arbeitsblatt
            workbook.CalculateFormula(calcOptions);

            // Erhalte das Ergebnis der Formel
            double result = worksheet.Cells["A2"].DoubleValue;

            // Gib das Ergebnis aus
            Console.WriteLine("Calculated Result: " + result);

            // Speichere die Arbeitsmappe
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


