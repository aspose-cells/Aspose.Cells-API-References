---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Sayfa adının tek tırnak içinde olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Sayfa adının tek tırnak içinde olup olmayacağını gösterir.

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | String | Sayfanın adı |

### Örnekler

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

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


