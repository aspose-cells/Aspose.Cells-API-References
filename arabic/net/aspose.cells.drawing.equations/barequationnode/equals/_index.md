---
title: "BarEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة BarEquationNode. تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيلين من BarEquationNode للمقارنة
            // ملاحظة: إنشاء BarEquationNode الفعلي سيعتمد على طرق المصنع في الـ API
            // للتوضيح، سنفترض أن هذه المثيلات مهيأة بشكل صحيح
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // قارن node1 بـ node2 (يجب أن تكون مساوية)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // قارن node1 بـ node3 (يجب ألا تكون مساوية)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // قارن node1 بـ null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // قارن node1 بنوع كائن مختلف
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // طريقة مساعدة لتوضيح الحصول على BarEquationNode
        // في الاستخدام الفعلي، ستستخدم طريقة API المناسبة لإنشاء هذه
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // هذا مجرد عنصر نائب - التنفيذ الفعلي سيعتمد على API
            // على سبيل المثال، قد يتم إنشاؤه عبر كائن أب أو طريقة مصنع
            return null; // Replace with actual creation code
        }
    }
}
```

### انظر أيضًا

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


