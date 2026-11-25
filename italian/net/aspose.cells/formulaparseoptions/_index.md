---
title: "Classe FormulaParseOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FormulaParseOptions. Rappresenta le opzioni durante l'analisi della formula"
type: docs
url: /it/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Rappresenta le opzioni durante l'analisi della formula.

```csharp
public class FormulaParseOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. Il valore predefinito è true (se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerato tale componente). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Definizione per l'analisi delle funzioni personalizzate. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Indica se la formula è formattata per la lingua locale. Il valore predefinito è false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Indica se analizzare la formula fornita. Il valore predefinito è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiama altri metodi per analizzarla o i dati della formula analizzata sono richiesti da altre operazioni, come il calcolo delle formule. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Indica se la formula utilizza lo stile di riferimento R1C1. Il valore predefinito è false. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Aggiungi una formula a una cella usando le opzioni
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Salva la cartella di lavoro
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


