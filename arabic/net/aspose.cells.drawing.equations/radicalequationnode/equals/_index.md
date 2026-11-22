---
title: "RadicalEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RadicalEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مثيلين من RadicalEquationNode
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // تعيين خصائص مختلفة لتوضيح مقارنة المساواة
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // قارن العقد باستخدام طريقة Equals
                bool areEqual = node1.Equals(node2);

                // اعرض نتيجة المقارنة
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // قارن مع نفس الكائن
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // قارن مع null
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


