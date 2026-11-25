---
title: "Workbook.ParseFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Analizza tutte le formule che non sono state analizzate quando sono state caricate da un file modello o impostate in una cella"
type: docs
url: /it/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate in una cella.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ignoreError | Booleano | Indica se ignorare l'errore per una formula non valida. Per una formula non valida, se si ignora l'errore la formula verrà ignorata e il processo continuerà ad analizzare le altre formule, altrimenti verrà sollevata un'eccezione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta le formule senza analisi (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Analizza tutte le formule in una volta
            wb.ParseFormulas(false);

            // Verifica le formule
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


