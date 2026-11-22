---
title: "Cell.GetPrecedentsInCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على جميع المراجع السابقة إلى الخلايا في المصنف الحالي المستخدمة في صيغة هذه الخلية أثناء حسابها"
type: docs
url: /ar/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

يحصل على جميع السلف (مرجع إلى خلايا في المصنف الحالي) التي تستخدمها صيغة هذه الخلية أثناء حسابها.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### قيمة الإرجاع

المعدِّد لتعداد جميع المراجع (ReferredArea)

### ملاحظات

يمكن لهذه الطريقة العمل فقط عندما تكون الخاصية [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) مضبوطة على true للمصنف وقد تم حساب المصنف بالكامل. إذا لم تكن هذه الخلية صيغة أو لم تُشر إلى أي خلايا أخرى، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


