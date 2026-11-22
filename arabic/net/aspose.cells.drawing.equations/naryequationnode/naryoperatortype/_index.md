---
title: "NaryEquationNode.NaryOperatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "NaryEquationNode property. معامل nary. على سبيل المثال"
type: docs
url: /ar/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

عامل n-ary. على سبيل المثال "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاحتواء المعادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // الوصول إلى المعادلة وإضافة عقدة معامل nary
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // تحويل إلى NaryEquationNode للوصول إلى NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // عرض NaryOperatorType الحالي (القيمة الافتراضية)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // تعيين إلى معامل الجمع (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // إضافة قاعدة (معامل) والحدود لتوضيح المعامل
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // تعيين المعامل لينمو مع محتواه
            naryEquationNode.NaryGrow = true;

            // تغيير إلى معامل الضرب (∏) وإظهار الفرق
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // احفظ المصنف
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


