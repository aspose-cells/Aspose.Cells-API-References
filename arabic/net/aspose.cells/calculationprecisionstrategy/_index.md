---
title: "تعداد CalculationPrecisionStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.CalculationPrecisionStrategy. يعدد الاستراتيجيات للتعامل مع دقة الحساب. بسبب مشكلة الدقة في حسابات IEEE 754 للعدد العائم قد لا يتم حساب بعض الصيغ البسيطة كما هو متوقع. مثل الصيغة 0.450.430.02 عند حساب المعاملات بواسطة العامل مباشرة النتيجة ليست صفرًا. لهذه المشكلة قد تعطي بعض الاستراتيجيات الخاصة النتيجة المتوقعة."
type: docs
url: /ar/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

يسرد استراتيجيات التعامل مع دقة الحساب. بسبب مشكلة الدقة في حسابات النقطة العائمة IEEE 754، قد لا تُحسب بعض الصيغ "التي تبدو بسيطة" بالنتيجة المتوقعة. مثل الصيغة "=-0.45+0.43+0.02"، عند حساب المعاملات باستخدام عامل '+' مباشرةً، النتيجة ليست صفرًا. بالنسبة لهذا النوع من مشاكل الدقة، قد توفر بعض الاستراتيجيات الخاصة النتيجة المتوقعة.

```csharp
public enum CalculationPrecisionStrategy
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لم يتم تطبيق أي استراتيجية على الحساب. عند الحساب استخدم القيمة المزدوجة الأصلية كمعامل وأعد النتيجة مباشرة. الأكثر كفاءة للأداء ومطبق على معظم الحالات. |
| Round | `1` | يقوم بتقريب نتيجة الحساب وفقًا للأرقام ذات الدلالة. |
| Decimal | `2` | يستخدم العشري كمعاملات عندما يكون ذلك ممكنًا. الأكثر غير كفاءة من حيث الأداء. |

### أمثلة

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // عيّن خيارات الحساب
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // احسب الصيغ في ورقة العمل.
            workbook.CalculateFormula(calcOptions);

            // احصل على نتيجة الصيغة.
            double result = worksheet.Cells["A2"].DoubleValue;

            // أخرج النتيجة.
            Console.WriteLine("Calculated Result: " + result);

            // احفظ المصنف
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


