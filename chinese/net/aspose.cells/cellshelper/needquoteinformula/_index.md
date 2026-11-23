---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsHelper 方法。指示工作表名称是否应使用单引号括起来"
type: docs
url: /zh/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

指示工作表名称是否应使用单引号括起来

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | String | 工作表的名称 |

### 示例

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

### 另请参见

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


