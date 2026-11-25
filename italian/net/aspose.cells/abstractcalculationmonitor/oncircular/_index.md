---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractCalculationMonitor. Implementa questo metodo per eseguire operazioni durante il calcolo di formule con riferimenti circolari"
type: docs
url: /it/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implementa questo metodo per gestire la logica di business durante il calcolo delle formule con riferimenti circolari.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator con elementi [`CalculationCell`](../../calculationcell/) che rappresentano celle dipendenti da riferimenti circolari. |

### Valore di ritorno

Indica se il motore di calcolo deve calcolare quelle celle in modo circolare dopo questa chiamata. True per consentire al motore di calcolo di continuare a calcolare per esse. False per far sì che il motore di calcolo le segni semplicemente come Calcolate.

### Osservazioni

Nell'implementazione l'utente può anche impostare il valore atteso come risultato calcolato per parte/tutte quelle celle, così il motore di calcolo non le calcolerà ricorsivamente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno scenario di riferimento circolare
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


