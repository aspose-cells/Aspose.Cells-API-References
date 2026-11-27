---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Anger om namnet på bladet ska omges av enkla citattecken"
type: docs
url: /sv/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Anger om bladnamnet ska omges av enkla citattecken

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | String | Namnet på bladet |

### Exempel

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

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


