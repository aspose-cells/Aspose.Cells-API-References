---
title: "CalculationData.CalculatedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. تحصل أو تعين القيمة المحسوبة لهذه الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

يحصل أو يضبط القيمة المحسوبة لهذه الدالة.

```csharp
public object CalculatedValue { get; set; }
```

### ملاحظات

يجب على المستخدم تعيين هذه الخاصية في محرك الحساب المخصص الخاص به للوظائف التي يدعمها المحرك، وسيتم إرجاع القيمة المعينة عند الحصول على هذه الخاصية لاحقًا. قد تكون القيمة المعينة من الأنواع الممكنة لـ [`Value`](../../cell/value/)، أو مصفوفة من مثل هذه القيم، أو نطاق (Range)، أو اسم (Name)، أو منطقة مُشار إليها (ReferredArea). الحصول على هذه الخاصية قبل تعيين قيمة لها سيجعل الدالة تُحسب بواسطة محرك الحساب الافتراضي في Aspose.Cells ثم تُرجع القيمة المحسوبة (عادةً ما تكون #NAME? للوظائف المعرفة من قبل المستخدم).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // إنشاء خيارات الحساب باستخدام محرك مخصص
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // حساب الصيغ مع خيارات
            workbook.CalculateFormula(options);

            // الحصول على القيمة المحسوبة
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


