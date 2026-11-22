---
title: "EquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/equals/
---
## EquationNode.Equals method

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

    public class EquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء عقدتي معادلة للمقارنة
            EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

            try
            {
                // استدعاء طريقة Equals مع معامل Object
                bool areEqual = node1.Equals((object)node2);

                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // تعديل node2 لجعلها مختلفة
                node2.AddChild(EquationNodeType.Base);

                areEqual = node1.Equals((object)node2);
                Console.WriteLine($"After modification, are they equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("EquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


