---
title: "EquationNode.InsertChild"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تُدرج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

يدرج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | قيمة الفهرس |
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

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
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
                // إضافة عقدة نصية أولية إلى المعادلة
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // إدراج عقدة كسر جديدة في الفهرس 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // احفظ المصنف
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


