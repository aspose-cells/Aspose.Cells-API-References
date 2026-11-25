---
title: "CellsHelper.AddAddInFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Aggiungi funzione add-in"
type: docs
url: /it/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Aggiungi funzione add-in.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| funzione | String | Il nome della funzione. |
| minCountOfParameters | Int32 | Numero minimo di parametri richiesti da questa funzione |
| maxCountOfParameters | Int32 | Numero massimo di parametri consentiti da questa funzione. |
| paramersType | ParameterType[] | Il tipo di parametri previsto della funzione |
| functionValueType | ParameterType | Il tipo di valore della funzione. |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare i metodi WorksheetCollection.RegisterAddInFunction(). Questo metodo sarà rimosso tra 12 mesi a partire da gennaio 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Definisci i parametri per AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Chiama il metodo AddAddInFunction
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Usa la funzione personalizzata in una cella
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Calcola le formule
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


