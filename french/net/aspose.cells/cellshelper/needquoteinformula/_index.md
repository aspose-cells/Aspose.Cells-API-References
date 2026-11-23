---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Indique si le nom de la feuille doit être entouré de guillemets simples"
type: docs
url: /fr/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Indique si le nom de la feuille doit être entouré de guillemets simples.

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | String | Le nom de la feuille |

### Exemples

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

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


