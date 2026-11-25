---
title: "FormulaParseOptions.Parse"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaParseOptions. Indica se analizzare la formula fornita. Il valore predefinito è true. Se è false, la stringa della formula rimarrà invariata per la cella finché l'utente non chiamerà altri metodi per analizzarla o finché i dati della formula analizzata non siano richiesti da altre operazioni, come il calcolo delle formule."
type: docs
url: /it/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Indica se analizzare la formula fornita. Il valore predefinito è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiama altri metodi per analizzarla o i dati della formula analizzata sono richiesti da altre operazioni, come il calcolo delle formule.

```csharp
public bool Parse { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta le formule con Parse=false (le formule non verranno analizzate immediatamente)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Calcola le formule (l'analisi avverrà ora)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


