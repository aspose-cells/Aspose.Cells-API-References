---
title: "TextParagraph.RightMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد الهامش الأيمن للفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

يحدد الهامش الأيمن للفقرة.

```csharp
public double RightMargin { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // الحصول على فقرة النص من الفقرة الأولى لمربع النص
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // اعرض قيمة الهامش الأيمن الحالية
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // عيّن قيمة جديدة للهامش الأيمن (بالنقاط)
            paragraph.RightMargin = 20.0;

            // أضف مربع نص آخر لإظهار الفرق
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // حفظ المصنف لرؤية التأثير
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


