---
title: "CalculationOptions.CalcStackSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200"
type: docs
url: /ar/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200.

```csharp
public int CalcStackSize { get; set; }
```

### ملاحظات

عند وجود عدد كبير من الخلايا تحتاج إلى حسابها بشكل متكرر في شجرة الاعتماد، قد يحدث استثناء StackOverflowException أثناء عملية الحساب. إذا حدث ذلك، يجب على المستخدم تحديد قيمة أصغر لهذه الخاصية. في مثل هذه الحالة، يجب على المستخدم تحديد القيمة المناسبة لهذه الخاصية وفقًا للصيغ والبيانات الفعلية. ومع ذلك، قد تتسبب القيمة الصغيرة جدًا في تدهور الأداء لحساب الصيغ، والقيمة الأقل من 2 تجعل من المستحيل حساب صيغة تعتمد على أخرى. لذلك إذا كانت القيمة المحددة أقل من 2، سيتم إعادة ضبطها إلى 2.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // إعداد صيغ نموذجية تتطلب حساب المكدس
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // احسب باستخدام حجم مكدس مخصص
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


