---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de CellsHelper. Indica si el nombre de la hoja debe estar entre comillas simples"
type: docs
url: /es/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Indica si el nombre de la hoja debe estar entre comillas simples

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | String | El nombre de la hoja |

### Ejemplos

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

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


