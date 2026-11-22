---
title: "Cell.GetDependentsInCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| recursive | منطقي | ما إذا كان يُرجع تلك التبعيات التي لا تشير إلى هذه الخلية مباشرةً بل تشير إلى فروع أخرى لهذه الخلية |

### قيمة الإرجاع

المُعدد لتعداد جميع التبعيات (كائنات Cell)

### ملاحظات

لاستخدام هذه الطريقة، يرجى التأكد من أن المصنف تم تعيينه بالقيمة true للخاصية [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) وتم حسابه بالكامل باستخدام هذا الإعداد. إذا لم يكن هناك إشارة صيغة إلى هذه الخلية، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


