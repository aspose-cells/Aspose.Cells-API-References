---
title: "التعداد EquationVerticalJustificationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType. يحدد هذا المحاذاة العمودية الافتراضية للمعادلات في المستند"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationverticaljustificationtype/
---
## EquationVerticalJustificationType enumeration

هذا يحدد المحاذاة العمودية الافتراضية للمعادلات في المستند.

```csharp
public enum EquationVerticalJustificationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Top | `0` | أعلى |
| Center | `1` | وسط |
| Bottom | `2` | أسفل |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationVerticalJustificationTypeDemo
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

            // تعيين خصائص المصفوفة
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // إضافة صفوف وأعمدة المصفوفة
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // احفظ المصنف
            string outputPath = "EquationVerticalJustificationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("File saved with vertical justification demo: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


