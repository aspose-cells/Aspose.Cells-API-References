---
title: "EquationNode.CreateNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. إنشاء عقدة من النوع المحدد"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

إنشاء عقدة من النوع المحدد.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | EquationNodeType | أنواع عقد المعادلة |
| المصنف | المصنف | كائن دفتر العمل المرتبط بالمعادلة |
| الأصل | EquationNode | العقدة الأصلية التي تقع فيها هذه العقدة |

### قيمة الإرجاع

إذا كان النوع المحدد موجودًا، يتم إرجاع العقدة المقابلة، وإذا لم يكن النوع موجودًا، يتم إرجاع عقدة من نوع غير معروف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل معادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // إنشاء عقدة أصلية (كسر)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // إنشاء عقدة البسط والعقدة المقام
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // إضافة الكسر المُنشأ إلى المعادلة الرئيسية
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // عرض المعادلة في خلية
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


