---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Indica se il nome del foglio deve essere racchiuso tra virgolette singole"
type: docs
url: /it/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Indica se il nome del foglio deve essere racchiuso tra virgolette singole.

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | String | Il nome del foglio |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodNeedQuoteInFormulaWithStringDemo
    {
        public static void Run()
        {
            Console.WriteLine("NeedQuoteInFormula(\"Test Ab\"): " + CellsHelper.NeedQuoteInFormula("Test Ab"));
            Console.WriteLine("NeedQuoteInFormula(\"A123\"): " + CellsHelper.NeedQuoteInFormula("A123"));
            Console.WriteLine("NeedQuoteInFormula(\"Sheet1\"): " + CellsHelper.NeedQuoteInFormula("Sheet1"));
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


