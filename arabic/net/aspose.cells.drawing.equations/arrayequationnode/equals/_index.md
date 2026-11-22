---
title: "ArrayEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ArrayEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/arrayequationnode/equals/
---
## ArrayEquationNode.Equals method

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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class ArrayEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء عقدتين معادلة من نوع المصفوفة
            ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
            ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // إضافة عقد فرعية لجعلها مختلفة
            EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
            // استخدم ToLaTeX() أو ToMathML() بدلاً من خاصية Value
            arrayEquation1.AddChild(child1);

            EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
            arrayEquation2.AddChild(child2);

            try
            {
                // استدعاء طريقة Equals مع كائنات مختلفة
                bool result1 = arrayEquation1.Equals(arrayEquation2);
                Console.WriteLine($"Comparing different array equations: {result1}");

                // استدعاء Equals مع نفس الكائن
                bool result2 = arrayEquation1.Equals(arrayEquation1);
                Console.WriteLine($"Comparing same array equation: {result2}");

                // استدعاء Equals مع قيمة null
                bool result4 = arrayEquation1.Equals(null);
                Console.WriteLine($"Comparing with null: {result4}");
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


