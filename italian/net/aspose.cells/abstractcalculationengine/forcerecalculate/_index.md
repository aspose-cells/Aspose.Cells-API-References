---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractCalculationEngine. Indica se forzare la ricalcolazione della funzione data ogni volta durante il calcolo delle formule condivise"
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Indica se forzare la ricomputazione della funzione specificata ogni volta durante il calcolo delle formule condivise.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionName | String | nome della funzione. Generalmente è il nome della funzione personalizzata. Se [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) è true, allora anche le funzioni integrate saranno verificate qui. |

### Valore di ritorno

true se la funzione specificata deve essere ricalcolata sempre.

### Osservazioni

Per le formule condivise, più celle condividono la stessa funzione. Se i parametri della funzione rimangono gli stessi per quelle celle, generalmente questa funzione deve essere calcolata solo una volta. Pertanto, per motivi di prestazioni, calcoliamo questo tipo di funzione una sola volta anche ([`Calculate`](../calculate/) viene chiamato una sola volta, invece di essere chiamato ripetutamente per ogni cella). Tuttavia, per l'implementazione personalizzata dell'utente, potrebbe essere necessario calcolare la funzione, in particolare la funzione personalizzata, in modo diverso per celle diverse. In tal caso, l'utente deve sovrascrivere questo metodo per farlo restituire true per la funzione. E per [`Calculate`](../calculate/), il valore [`CalculatedValue`](../../calculationdata/calculatedvalue/) fornito potrebbe essere stato inizializzato con il valore memorizzato nella cache del calcolo precedente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


