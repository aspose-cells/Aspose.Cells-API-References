---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomFunctionDefinition. Ottiene gli indici dei parametri delle funzioni personalizzate forniti che devono essere calcolati in modalità array"
type: docs
url: /it/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Restituisce gli indici dei parametri della funzione personalizzata fornita che devono essere calcolati in modalità array.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionName | String | Nome della funzione personalizzata. |

### Valore di ritorno

Indici dei parametri che devono essere calcolati in modalità array per la funzione personalizzata fornita. Il valore predefinito è null, non esiste alcun parametro che debba essere calcolato in modalità array per la funzione personalizzata.

### Osservazioni

Per un'espressione che deve essere calcolata, prendendo A:A+B:B come esempio: generalmente in modalità valore verrà calcolata a un singolo valore in base alla cella corrente. Ma in modalità array, tutti i valori di A1+B1, A2+B2, A3+B3, ... verranno calcolati e utilizzati per il calcolo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Chiama GetArrayModeParameters con un parametro nome della funzione
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Visualizza il risultato
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


