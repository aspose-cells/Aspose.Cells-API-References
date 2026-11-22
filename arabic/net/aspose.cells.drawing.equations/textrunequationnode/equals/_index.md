---
title: "TextRunEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextRunEquationNode. تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // لأغراض العرض، سنستخدم null وسنظهر فقط منطق المقارنة
            // نظرًا لأنه لا يمكننا إنشاء مثيلات TextRunEquationNode مباشرة
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // هذا الجزء يبقى لإظهار كيفية استدعاء Equals
                // في سيناريو حقيقي، ستكون هذه العقد مهيأة بشكل صحيح
                if (node1 != null && node2 != null && node3 != null)
                {
                    // قارن node1 مع node2 (نفس المحتوى)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // قارن node1 مع node3 (محتوى مختلف)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // قارن مع null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // قارن مع نوع كائن مختلف
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ دفتر العمل (على الرغم من أن Equals لا يعدل جدول البيانات)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // تم إزالة طريقة المساعدة نظرًا لأنه لا يمكننا إنشاء مثيلات TextRunEquationNode بشكل صحيح
    }
}
```

### انظر أيضًا

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


