---
title: "Cell.GetDependents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة الخلية. احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرة"
type: docs
url: /ar/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرةً.

```csharp
public Cell[] GetDependents(bool isAll)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isAll | منطقي | تشير إلى ما إذا كان يتم فحص الصيغ في أوراق عمل أخرى |

### ملاحظات

إذا ظهر مرجع يحتوي على هذه الخلية في صيغة خلية ما، فسيُعتبر تلك الخلية تابعًا لهذه الخلية، بغض النظر عما إذا كان المرجع أو هذه الخلية يُستخدم أثناء الحساب أم لا. على سبيل المثال، رغم أن الخلية A2 في الصيغة "=IF(TRUE,A1,A2)" لا تُستخدم أثناء الحساب، إلا أن هذه الصيغة لا تزال تُعتبر تابعًا للخلية A2. للحصول على تلك الصيغ التي تعتمد نتائجها المحسوبة على هذه الخلية، يرجى استخدام [`GetDependentsInCalculation`](../getdependentsincalculation/). عند تتبع التوابع لخلية واحدة، سيتم تحليل جميع الصيغ في المصنف أو ورقة العمل وفحصها. لذا فإن العملية تستغرق وقتًا. إذا كان المستخدم يحتاج إلى تتبع التوابع لعدد كبير من الخلايا، فإن استخدام هذه الطريقة سيتسبب في أداء ضعيف. لأسباب تتعلق بالأداء، يجب على المستخدم استخدام [`GetDependentsInCalculation`](../getdependentsincalculation/) بدلاً من ذلك. أو قد يجمع المستخدم خريطة السلف لجميع الخلايا باستخدام [`GetPrecedents`](../getprecedents/) أولاً، ثم يبني خريطة التوابع وفقًا لخريطة السلف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين الصيغ التي تشير إلى B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // حساب الصيغ
            workbook.CalculateFormula();

            // الحصول على جميع الخلايا التي تعتمد على B1 (متكرر)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


