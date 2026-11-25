---
title: "Classe CustomFunctionDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CustomFunctionDefinition. Definizione della funzione personalizzata per il calcolo con il motore personalizzato dell'utente"
type: docs
url: /it/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Definizione di funzione personalizzata per il calcolo con il motore personalizzato dell'utente.

```csharp
public class CustomFunctionDefinition
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Restituisce gli indici dei parametri della funzione personalizzata fornita che devono essere calcolati in modalità array. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea una nuova istanza di CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Crea una nuova istanza di FormulaParseOptions e imposta il CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Aggiungi un foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Definisci una formula personalizzata
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Analizza la formula personalizzata utilizzando FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Salva la cartella di lavoro
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


