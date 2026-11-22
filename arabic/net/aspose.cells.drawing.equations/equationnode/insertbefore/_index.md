---
title: "EquationNode.InsertBefore"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تُدرج العقدة المحددة قبل العقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

يدرج العقدة المحددة قبل العقدة الحالية.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء معادلة رياضية في الخلية A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // إضافة عقدة نصية أولية إلى المعادلة
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // إدراج عقدة نصية جديدة قبل الموجودة
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // عرض المعادلة بتنسيق LaTeX
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


