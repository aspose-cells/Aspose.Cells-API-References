---
title: "EquationNodeParagraph.Justification"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية EquationNodeParagraph. تحدد محاذاة الفقرة الرياضية، وهي سلسلة من المعادلات المتجاورة داخل نفس الفقرة. يمكن أن تكون الفقرة الرياضية محاذاة إلى اليسار أو إلى اليمين أو مركزية أو مركزية كمجموعة. بشكل افتراضي تكون الفقرة الرياضية مركزية كمجموعة. هذا يعني أن المعادلات يمكن محاذاتها بالنسبة لبعضها البعض لكن المجموعة الكاملة من المعادلات تكون مركزية ككل."
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

هذا يحدد محاذاة الفقرة الرياضية (سلسلة من المعادلات المتجاورة داخل نفس الفقرة). يمكن أن تكون الفقرة الرياضية محاذاة إلى اليسار، أو إلى اليمين، أو في الوسط، أو في الوسط كمجموعة. بشكل افتراضي، تكون الفقرة الرياضية في الوسط كمجموعة. وهذا يعني أن المعادلات يمكن محاذاتها بالنسبة لبعضها، لكن المجموعة الكاملة من المعادلات تكون في الوسط ككل.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاحتواء المعادلة
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // احصل على فقرة المعادلة
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // عرض قيمة المحاذاة الحالية
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // تعيين قيم محاذاة مختلفة وملاحظة التأثيرات
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // احفظ المصنف
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


