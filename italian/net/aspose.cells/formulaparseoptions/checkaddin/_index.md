---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaParseOptions. Indica se verificare gli add-in nei collegamenti esterni esistenti della cartella di lavoro corrente per funzioni definite dall'utente senza collegamento esterno. Il valore predefinito è true; se la funzione definita dall'utente corrisponde a un add-in nei collegamenti esterni esistenti, viene considerata come tale add-in."
type: docs
url: /it/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per le funzioni definite dall'utente senza collegamento esterno. Il valore predefinito è true (se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerato tale componente).

```csharp
public bool CheckAddIn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Registra la funzione add-in
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Senza CheckAddIn=false - la formula verrà convertita nel formato add-in
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // Con CheckAddIn=false - la formula rimane invariata
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


