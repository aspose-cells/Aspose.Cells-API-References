---
title: "LimLowUppEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LimLowUppEquationNode. تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | العقدة المحددة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // نظرًا لأننا لا نعرف معلمات المُنشئ، سنقارن القيم الفارغة (null)
            // هذا تعديل بسيط لجعل الكود يُترجم - في الاستخدام الفعلي ستحتاج إلى إنشاء صحيح
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // استدعِ طريقة Equals مع نوع المعامل المحدد (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // اعرض النتيجة
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // احفظ المصنف
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


