---
title: "CellsHelper.NeedQuoteInFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تشير إلى ما إذا كان يجب إحاطة اسم الورقة بعلامات اقتباس مفردة"
type: docs
url: /ar/net/aspose.cells/cellshelper/needquoteinformula/
---
## CellsHelper.NeedQuoteInFormula method

يحدد ما إذا كان يجب إغلاق اسم الورقة بين علامات اقتباس مفردة

```csharp
public static bool NeedQuoteInFormula(string sheetName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | String | اسم الورقة |

### أمثلة

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

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


