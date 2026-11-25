---
title: "CalculationData.CalculatedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Restituisce o imposta il valore calcolato per questa funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Ottiene o imposta il valore calcolato per questa funzione.

```csharp
public object CalculatedValue { get; set; }
```

### Osservazioni

L'utente dovrebbe impostare questa proprietà nel proprio motore di calcolo personalizzato per le funzioni supportate dal motore, e il valore impostato verrà restituito quando si legge nuovamente la proprietà. Il valore impostato può essere di uno dei possibili tipi di [`Value`](../../cell/value/), o un array di tali valori, oppure un Range, un Name, un ReferredArea. Leggere questa proprietà prima di aver impostato un valore farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e quindi verrà restituito il valore calcolato (in genere dovrebbe essere #NAME? per le funzioni definite dall'utente).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Crea opzioni di calcolo con motore personalizzato
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Calcola le formule con opzioni
            workbook.CalculateFormula(options);

            // Ottenere il valore calcolato
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


