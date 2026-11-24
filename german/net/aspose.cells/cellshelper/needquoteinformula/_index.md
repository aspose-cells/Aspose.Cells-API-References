---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll"
type: docs
url: /de/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll.

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | String | Der Name des Blattes |

### Beispiele

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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


