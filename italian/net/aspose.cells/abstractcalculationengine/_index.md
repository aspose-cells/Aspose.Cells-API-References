---
title: "Classe AbstractCalculationEngine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractCalculationEngine. Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells"
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di **Aspose.Cells**.

```csharp
public abstract class AbstractCalculationEngine
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) è richiesto durante il calcolo di funzioni personalizzate e l'utente non ha aggiornato la definizione per esse (tramite [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), questa proprietà deve essere impostata su true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Indica se questo motore necessita del testo letterale del parametro durante un calcolo. Il valore predefinito è false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Indica se le funzioni integrate supportate dal motore integrato debbano essere verificate ed elaborate da questa implementazione. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Calcola una funzione con i dati forniti. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Indica se forzare la ricomputazione della funzione specificata ogni volta durante il calcolo delle formule condivise. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione. |

### Osservazioni

L'utente non dovrebbe modificare direttamente alcuna parte della Cartella di lavoro in questa implementazione (eccetto il risultato calcolato della funzione personalizzata, che può essere impostato tramite la proprietà CalculationData.CalculatedValue). Altrimenti potrebbero verificarsi risultati inattesi o eccezioni. Se l'utente ha bisogno di modificare altri dati oltre al risultato calcolato nell'implementazione per alcune funzioni personalizzate, ad esempio modificare la formula di una cella, lo stile, ...ecc., l'utente dovrebbe raccogliere tali dati in questa implementazione e modificarli al di fuori dell'ambito del calcolo della formula.

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Esempio: Implementazione personalizzata per una funzione denominata "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Supponendo che MYFUNC accetti due parametri e restituisca la loro somma
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Forza la ricomputazione per la funzione personalizzata "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Inserisci alcuni valori nelle celle
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Aggiungi una formula che utilizza la funzione personalizzata
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Imposta le opzioni di calcolo con il motore personalizzato
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Calcola le formule con il motore personalizzato
            workbook.CalculateFormula(options);

            // Stampa il risultato della funzione personalizzata
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Salva la cartella di lavoro
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


