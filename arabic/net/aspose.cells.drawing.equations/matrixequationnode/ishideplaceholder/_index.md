---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MatrixEquationNode. تُحدد هذه السمة خاصية إخفاء العناصر النائبة على المصفوفة. عندما تكون هذه الخاصية مفعلة لا تظهر العناصر النائبة في المصفوفة. بشكل افتراضي تظهر العناصر النائبة بحيث تكون المواقع التي يمكن إدراج النص فيها مرئية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

تحدد هذه الخاصية خاصية إخفاء العناصر النائبة في المصفوفة. عندما تكون هذه الخاصية مفعلة، لا تظهر العناصر النائبة في المصفوفة. بشكل افتراضي، تظهر العناصر النائبة بحيث تكون المواقع التي يمكن إدراج النص فيها مرئية.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على عقدة الرياضيات وأضف المصفوفة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // تعيين خصائص المصفوفة
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // أضف مصفوفة 2×2 ذات القطر مكوّن من 1
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // حفظ والتحقق
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


