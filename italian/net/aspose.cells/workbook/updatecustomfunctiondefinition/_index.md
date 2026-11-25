---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Aggiorna la definizione delle funzioni personalizzate"
type: docs
url: /it/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Aggiorna la definizione delle funzioni personalizzate.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| definizione | CustomFunctionDefinition | Definizione speciale delle funzioni personalizzate per la specifica esigenza dell'utente. |

### Osservazioni

Questo metodo può essere utilizzato in alcuni scenari speciali. Ad esempio, se l'utente ha bisogno che alcuni parametri di alcune funzioni personalizzate vengano calcolati in modalità array, allora l'utente può fornire la propria definizione con il metodo implementato [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) per quelle funzioni. Dopo l'aggiornamento dei dati delle formule, i parametri specificati saranno calcolati automaticamente in modalità array durante il calcolo delle funzioni personalizzate corrispondenti.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Crea un motore di calcolo personalizzato
            var customEngine = new MyCustomCalculationEngine();
            
            // Imposta le opzioni di calcolo con motore personalizzato
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Aggiorna la definizione della funzione personalizzata
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Imposta la formula usando la funzione personalizzata
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Calcola le formule
            wb.CalculateFormula(options);

            // Restituisci il risultato
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Restituisce gli indici dei parametri che devono essere elaborati in modalità array
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Vedi anche

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


