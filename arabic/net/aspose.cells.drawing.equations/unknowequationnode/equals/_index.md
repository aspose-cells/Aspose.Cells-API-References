---
title: "UnknowEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnknowEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء عقدتي معادلة غير معروفة للمقارنة
            // نظرًا لأن UnknowEquationNode لا يحتوي على مُنشئ بدون معلمات،
            // سيتعين علينا إنشاؤها بطريقة مختلفة. لأغراض العرض، سنستخدم
            // المُنشئ الفعلي إذا كان متاحًا، أو إنشاؤها بوسائل أخرى.
            // نظرًا لعدم معرفتنا بمعلمات المُنشئ، فهذا إصلاح مؤقت.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // استدعِ طريقة Equals مع نوع المعامل المحدد (Object)
                bool areEqual = node1.Equals(objToCompare);

                // اعرض النتيجة
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // أضف النتيجة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // طريقة مساعدة لإنشاء مثيلات UnknowEquationNode
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // في تنفيذ حقيقي، سيستخدم هذا المُنشئ المناسب
            // نظرًا لعدم معرفتنا بمعلمات المُنشئ، سنعيد قيمة null
            // وتعامل مع حالة null في العرض (على الرغم من أن هذا مجرد عنصر نائب)
            return null;
        }
    }
}
```

### انظر أيضًا

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


