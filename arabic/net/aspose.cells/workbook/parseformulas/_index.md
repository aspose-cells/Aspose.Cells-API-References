---
title: "Workbook.ParseFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحلل جميع الصيغ التي لم يتم تحليلها عند تحميلها من ملف القالب أو تعيينها إلى خلية"
type: docs
url: /ar/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

يقوم بتحليل جميع الصيغ التي لم يتم تحليلها عندما تم تحميلها من ملف القالب أو تعيينها إلى خلية.

```csharp
public void ParseFormulas(bool ignoreError)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ignoreError | منطقي | ما إذا كان سيتم تجاهل الخطأ للمعادلة غير الصالحة. بالنسبة لمعادلة غير صالحة واحدة، إذا تم تجاهل الخطأ فسيتم تجاهل هذه المعادلة وسيستمر العملية في تحليل المعادلات الأخرى، وإلا سيتم إلقاء استثناء. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين الصيغ دون التحليل (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // تحليل جميع الصيغ مرة واحدة
            wb.ParseFormulas(false);

            // تحقق من الصيغ
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


