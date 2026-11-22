---
title: "MatrixEquationNode.BaseJc"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MatrixEquationNode. تُحدد هذه السمة محاذاة المصفوفة. يمكن محاذاة النص خارج المصفوفة إلى الأسفل أو الأعلى أو وسط دالة المصفوفة. بشكل افتراضي، تفترض المصفوفة محاذاة مركزية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

تحدد هذه الخاصية محاذاة المصفوفة. يمكن محاذاة النص خارج المصفوفة إلى الأسفل أو الأعلى أو الوسط لوظيفة المصفوفة. بشكل افتراضي، تفترض المصفوفة محاذاة مركزية.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyBaseJcDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة شكل معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على فقرة المعادلة وأضف عقدة مصفوفة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // تعيين خصائص المصفوفة بما في ذلك BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Add 2x2 matrix content (identity matrix)
            for (int row = 0; row < 2; row++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // احفظ المصنف
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### انظر أيضًا

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


