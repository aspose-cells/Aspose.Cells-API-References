---
title: "EquationNode.RemoveAllChildren"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تُزيل جميع العقد الفرعية للعقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/removeallchildren/
---
## EquationNode.RemoveAllChildren method

يزيل جميع العقد الفرعية للعقدة الحالية.

```csharp
public void RemoveAllChildren()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveAllChildrenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاحتواء المعادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // الحصول على عقدة المعادلة
            var equationNode = ((TextBox)shape).GetEquationParagraph();

            // إضافة بعض العقد الفرعية إلى المعادلة
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML

            Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");

            try
            {
                // استدعاء طريقة RemoveAllChildren
                equationNode.RemoveAllChildren();

                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


