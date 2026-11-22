---
title: "EquationNode.InsertAfter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تُدرج العقدة المحددة بعد العقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

يدرج العقدة المحددة بعد العقدة الحالية.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | EquationNodeType | أنواع عقد المعادلة |

### قيمة الإرجاع

إذا كان النوع المحدد موجودًا، يتم إرجاع العقدة المقابلة، وإذا لم يكن النوع موجودًا، يتم إرجاع عقدة من نوع غير معروف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل معادلة في الخلية A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // إضافة عقدة نصية أولية
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // إدراج عقدة نصية جديدة بعد العقدة الحالية
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // عرض بنية المعادلة
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // حفظ المعادلة في خلية للتفحص البصري
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


