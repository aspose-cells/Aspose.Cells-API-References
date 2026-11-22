---
title: "FractionEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FractionEquationNode. تحدد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // نظرًا لأن FractionEquationNode لا يحتوي على مُنشئ بدون معلمات،
                // سنوضح طريقة Equals باستخدام كائنات من المفترض أنها تأتي من أجزاء أخرى في API
                // لأغراض العرض، سنفترض أن لدينا مثيلين للمقارنة
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // قارن الكائنات باستخدام Equals
                bool areEqual = node1.Equals(node2);

                // اعرض نتيجة المقارنة
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // قارن مع null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // قارن مع نفسه
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // طريقة مساعدة لمحاكاة الحصول على مثيلات FractionEquationNode
        // (في الاستخدام الفعلي، هذه ستأتي من API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // هذا مجرد عنصر نائب - في الواقع ستحصل على هذه من API
            // على سبيل المثال: worksheet.Equations.AddFractionEquationNode() أو ما شابه
            return null; // Actual implementation would depend on API
        }
    }
}
```

### انظر أيضًا

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


