---
title: "MathematicalEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة MathematicalEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مثيلين من MathematicalEquationNode للمقارنة
                // نظرًا لأن MathematicalEquationNode لا يحتوي على مُنشئ بدون معلمات،
                // سنحتاج إلى تمرير null أو المعلمات المناسبة
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // قارن العقد باستخدام طريقة Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // اعرض نتيجة المقارنة
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // قارن مع نوع كائن مختلف
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
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

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


