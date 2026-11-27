---
title: "Workbook.ParseFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Tolkar alla formler som inte har tolkats när de lästes in från mallfil eller placerades i en cell"
type: docs
url: /sv/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes i en cell.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ignoreError | Boolean | Om fel för ogiltig formel ska ignoreras. För en ogiltig formel, om fel ignoreras så kommer denna formel att hoppas över och processen fortsätter att tolka andra formler, annars kastas ett undantag. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange formler utan tolkning (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Tolkar alla formler på en gång
            wb.ParseFormulas(false);

            // Verifiera formlerna
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


