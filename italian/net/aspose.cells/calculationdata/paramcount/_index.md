---
title: "CalculationData.ParamCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Restituisce il conteggio dei parametri"
type: docs
url: /it/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Ottiene il conteggio dei parametri

```csharp
public int ParamCount { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Popolare alcune celle che saranno usate come parametri
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Impostare una formula che chiama una funzione personalizzata con tre argomenti
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Configura le opzioni di calcolo per utilizzare un motore personalizzato
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Esegui il calcolo
                workbook.CalculateFormula(options);

                // Il motore personalizzato restituisce ParamCount come valore calcolato
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Salva opzionalmente la cartella di lavoro
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Motore di calcolo personalizzato che dimostra la lettura della proprietà ParamCount
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identifica la funzione personalizzata per nome
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Leggi la proprietà ParamCount in sola lettura
                    int count = data.ParamCount;

                    // Usa il conteggio come risultato della funzione
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


