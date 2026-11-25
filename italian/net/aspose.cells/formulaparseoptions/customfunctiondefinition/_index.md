---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaParseOptions. Definizione per l'analisi delle funzioni personalizzate"
type: docs
url: /it/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Definizione per l'analisi delle funzioni personalizzate.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Osservazioni

Per alcuni requisiti speciali, ad esempio quando si calcola una funzione personalizzata nel motore personalizzato dell'utente, alcuni parametri devono essere calcolati in modalità matrice; utilizzando questa proprietà è possibile contrassegnare tali parametri come modalità matrice durante l'analisi della formula. In caso contrario, l'utente deve aggiornare in seguito quelle funzioni personalizzate tramite [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) per ottenere lo stesso risultato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea la definizione della funzione personalizzata
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Configura le opzioni di analisi della formula con funzione personalizzata
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Utilizza la funzione personalizzata nella formula
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Calcola la cartella di lavoro per dimostrare l'elaborazione della funzione personalizzata
            workbook.CalculateFormula();

            // Salva il risultato
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


