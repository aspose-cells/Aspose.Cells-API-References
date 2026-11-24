---
title: "Workbook.ParseFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Analysiert alle Formeln, die beim Laden aus einer Vorlagendatei oder beim Setzen in eine Zelle nicht analysiert wurden"
type: docs
url: /de/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Parst alle Formeln, die beim Laden aus einer Vorlagendatei oder beim Setzen in eine Zelle nicht geparst wurden.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ignoreError | Boolean | Ob Fehler für ungültige Formeln ignoriert werden sollen. Für eine ungültige Formel, wenn Fehler ignoriert werden, wird diese Formel ignoriert und der Vorgang fährt fort, andere Formeln zu analysieren; andernfalls wird eine Ausnahme ausgelöst. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formeln ohne Analyse festlegen (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Alle Formeln auf einmal analysieren
            wb.ParseFormulas(false);

            // Überprüfen Sie die Formeln
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


