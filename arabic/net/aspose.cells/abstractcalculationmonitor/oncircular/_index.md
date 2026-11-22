---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractCalculationMonitor. نفّذ هذه الطريقة للقيام بالعمليات عند حساب الصيغ ذات المراجع الدائرية"
type: docs
url: /ar/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

نفّذ هذه الطريقة للقيام بالأعمال عند حساب الصيغ ذات المراجع الدائرية.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator مع عناصر [`CalculationCell`](../../calculationcell/) التي تمثل الخلايا التي تعتمد على المراجع الدائرية. |

### قيمة الإرجاع

ما إذا كان محرك الصيغ يحتاج إلى حساب تلك الخلايا في الدائرية بعد هذه الاستدعاء. True للسماح لمحرك الصيغ بالاستمرار في حسابها. False لجعل محرك الصيغ يضع علامة فقط على تلك الخلايا كـ Calculated.

### ملاحظات

في التنفيذ قد يقوم المستخدم أيضًا بتعيين القيمة المتوقعة كنتيجة محسوبة لجزء/كل تلك الخلايا بحيث لا يقوم محرك الصيغ بحسابها بشكل متكرر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء سيناريو مرجع دائري
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


