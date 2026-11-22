---
title: "BoxEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة BoxEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائنين من BoxEquationNode للمقارنة
            // نظرًا لأن BoxEquationNode لا يحتوي على مُنشئ بدون معلمات،
            // سنحتاج إلى إنشائهما بطريقة مختلفة. بافتراض أنه يمكننا الحصول عليهما من مكان ما،
            // أو إنشائهما ببعض المعلمات الافتراضية.
            // لأغراض العرض، سنقوم فقط بالإعلان عنها وتعيين null (على الرغم من أنه في الكود الفعلي ستحتاج إلى تهيئة صحيحة)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // استدعاء طريقة Equals مع أنواع المعلمات المحددة (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // اعرض النتيجة
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // أضف النتيجة إلى ورقة العمل
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // حفظ النتيجة
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


