---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Указывает, должно ли имя листа быть заключено в одинарные кавычки"
type: docs
url: /ru/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

Указывает, следует ли заключать имя листа в одинарные кавычки

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | String | Имя листа |

### Примеры

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

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


